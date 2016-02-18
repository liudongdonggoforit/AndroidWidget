package com.ldd.androidwidget;

import android.app.Activity;
import android.graphics.Typeface;
import android.os.Bundle;
import android.widget.Button;
import android.widget.TextView;

public class MainActivity extends Activity {

	private TextView customTv;
	@Override
	protected void onCreate(Bundle savedInstanceState) {
		super.onCreate(savedInstanceState);
		setContentView(R.layout.activity_main);
		//初始化控件
		initView();
	}
	//初始化控件
	private void initView() {
		customTv = (TextView) findViewById(R.id.Custom_TextView_Id);
		/**
		 * 必须事先在assets下创建一个fonts文件夹  并放入要使用的字体文件（.ttf  .TTF）
		 * 并提供相对路径给createFromAsset()来创建Typeface对象
		 */
		Typeface fontFace = Typeface.createFromAsset(getAssets(), "fonts/niutuku.ttf");
		/**
		 * 使用的字体格式必须是true type font 的格式 （ttf或者TTF）
		 * 当使用外部字体却又发现字体没有变化的时候（以Droid Sans代替），通常是因为这个字体Android没有支持，而非程序发了错误
		 */
		customTv.setTypeface(fontFace);
	}
}
