����֤��ר�����Я����(http://www.ctrip.com)��д,�����ڸ���վ��֤���ʶ��.

ʹ�÷����ܼ�,����������ʾ:

File modelFile = new File("model");
CtripCaptchaDecoder decoder = new CtripCaptChaDecoder(modelFile);

BufferedImage image = ImageIO.read(new File("test.jpg"));
String code = decoder.decode(image);

����: modelFile�Ǳ���Ԥ��ѵ���õı���ģʽ���ļ�(�ļ���Ϊmodel), image����������Я������֤��ͼƬ���Ӧ��BufferedImage;

����, ������������ڵ��߳�ʹ��; ������߳�ʹ��, ����ÿ���߳��ж�����һ��CtripCaptchaDecoder.