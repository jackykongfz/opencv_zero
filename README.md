
#include"highgui.h"
#include"stdio.h"

int main(int argc, char** argv)
{
	IplImage* img = cvLoadImage( "C:\\ps素材\\读书笔记.jpg",1 );//加载所指图片到内存
	cvNamedWindow("fuck first", CV_WINDOW_AUTOSIZE);//命名窗口
	cvShowImage("fuck first", img);//显示图像
	cvWaitKey(0);//等待键盘输入
	cvReleaseImage(&img);//释放内存
	cvDestroyWindow("fuck first");//摧毁窗口
}
