hexo-template-damien

hexo-template-damien�ǻ���hexo-theme-snippet������hexo����ģ�塣

���������ģ���ܰ������㣬�붯����ָ Star ֧��һ��

image image image image image image image

����Ч����ʾ

image

����ƪ

������ڴ�֮ǰʹ�õ��� Hexo 2.x �汾��Ϊ�˱���δ֪�Ĵ����뱸�ݺ����ݣ����߽����µĲ���Ŀ¼ "����Ŀ¼" => themes\hexo-theme-snippet, "Hexo��Ŀ¼" => ��Ŀ��Ŀ¼; "��������" => themes\hexo-theme-snippet_config.yml, "Hexo����" => ��Ŀ��Ŀ¼��_config.yml
�����

��ҪNode.js ������Git �����Լ� Hexo

����ģ��

�����ַ�ʽ��ȡ������--���� *.zip �ļ���ͨ�� git��ʽ��

����zip��

���ظ�ѹ���ļ�֮��ֱ�ӽ�ѹ���ɡ�

Git��ʽ

git clone https://github.com/damienzhong/hexo-template-damien.git
��װ���

������ĿĿ¼hexo-template-damien����Git Bashִ���������װ������

npm install hexo --save
�������δ��װ���߲��˽� Hexo����ο� �ٷ��̳� �����˽��Լ���װ��

npm i hexo-renderer-ejs hexo-renderer-less hexo-deployer-git -S
���𲩿�

���²���������Git Bash��ִ��

���hexo��̬�ļ��ͻ��棬����������

hexo clean && hexo g  //��ջ��沢���ɾ�̬�ļ�
����Ԥ����ȷû�������ٽ��з���

hexo s  //�������ط���Ĭ��
������github

hexo d ���� gulp deploy  //���𷢲�
����ƪ

��������

## menu -- �����˵���ʾ{[@page:����,@url:��ַ,@icon:ͼ��]}
menu:
  - page: home
    url: /
    icon: fa-home

## favicon -- ��վͼ��λ��{@favicon}
favicon: /favicon.ico

## rss --rss�ļ�λ��{@rss}
rss: /atom.xml


# ����С���ߵ�����

## widgets -- 6�����С����{@widgets:[notification,category,archive,tagcloud,friends]}
widgets:
  - search
  - notification
  - social
  - category
  - archive
  - tagcloud
  - friends

# ����С���ߵ�����

## ����
jsonContent:
  searchLocal: true // �Ƿ����ñ�������
  searchGoogle: true //�Ƿ����ùȸ�����
  posts:
    title: true
    text: true
    content: true
    categories: false
    tags: false

## notification config --��վ��������,֧�� html �� ���ı�
notification: |-
            <p>
                ֧�ֱ����ͣ�<a href="https://github.com/damienzhong/damienzhong.github.io/stargazers" title="star me" target="_blank">Starһ��</a> <br/>
                �ſᲥ����<a href="https://i.youku.com/i/UNDE3MDU5OTg3Mg==/playlists">�ſᲥ��</a><br/>
                �Ա���װ�꣺<a href="https://shop72495432.taobao.com/search.htm?spm=a1z10.1-c.0.0.25343b46cBwhQs&search=y">DM��������</a><br/>
                QQ����Ⱥ��<a href="https://jq.qq.com/?_wv=1027&k=5xgZ7E0" title="" target="_blank">�������Ⱥ�ġ������Ӽ�������Ⱥ��</a> 
            </p>

## �罻����{@name:�罻�������֣�@icon:�罻����ͼ�꣬@href:���ù�������} [�ο�ͼ��](http://fontawesome.io/icons/)
social:
  - name: Github
    icon: git
    href: //github.com/damienzhong

## ���·�������{@cate_config:{@show_count:�Ƿ���ʾ���֣�@show_current: �Ƿ������ǰcategory}}
cate_config:
   show_count: true
   show_current: true

## ���¹鵵����{@arch_config:/*�����ο���https://hexo.io/zh-cn/docs/helpers.html#list-archives*/}
## �Ƽ���Ϸ�ʽ��[{type: 'monthly',format: 'YYYY��MM��'},{type: 'yearly',format: 'YYYY��'}]
arch_config:
   type: 'monthly'
   format: 'YYYY��MM��'
   show_count: true
   order: -1

## ��ǩ������{/*�����ο���http://www.goat1000.com/tagcanvas-options.php */}
tagcloud:
  tag3d: false // �Ƿ�����3D��ǩ��
  textColour: '#444' // ������ɫ
  outlineMethod: 'block' // ѡ��ģʽ(outline|classic|block|colour|size|none)
  outlineColour: '#FFDAB9' // ѡ��ģʽ����ɫ
  interval: 30 // ����֮֡���ʱ������ֵԽ��ת������Խ��
  freezeActive: true // ѡ�еı�ǩ�Ƿ��������
  frontSelect: true // ��ѡ��ǩ�ƺ󲿵ı�ǩ
  reverse: true // �Ƿ��򴥷�
  wheelZoom: false // �Ƿ�����������

## ��������{@�������ƣ����ӵ�ַ{@links:[,,,]}}
links:
  - Hexo����: https://hexo.io/zh-cn/


# �����Զ�����Ի�����

## ��վ������{@branding����վ������(��������ʾ����ͼƬ)}
branding: ��δ��˼���Ȥ

## ����banner����ͼƬ{@img:imgUrl�Զ���ͼƬ��ַ,����Ĭ��{"��̬����":"banner.jpg"},{"��̬����":"banner2.jpg"}}
banner:
  img: imgUrl

## ����carousel{@img:ͼƬ��ַ,@url:�����ת����(Ĭ��ֵ:"javascript:")}
carousel:
  img: 'img/head-img.jpg'
  url: 'javascript:'

## ��ҳ�б�ײ����{@homePanel: �Ƿ���}
homePanel: true

## ��ҳ�����б�����ͼ
### ���ع���: �Զ�����������ͼ(��Front-matter����ӵ�'img'�ֶ�) > �����ڵ�ͼƬ > defaultImgs(�����ȡ) > ��ͼģʽ�б�

## �Զ������ͼƬ
defaultImgs:
  - http://www.example.jpg //Զ��ͼƬ����ʾ��
  - /img/default-1.jpg //����ͼƬ����ʾ��

### ����ժҪ{@ժҪ��ʾ���ȼ����Զ���ժҪ > �Զ���ȡժҪ }
### �Զ���ժҪ��Χ{@<!--more-->:��ȡmore֮ǰ������ΪժҪ}
### �Զ���ȡժҪ{@excerptLength:�Զ���ȡ����ǰ���ٸ���ΪժҪ��������Ĭ�ϣ�120��}
excerptLength: 120

## �Ƿ�������Ŀ¼
toc: true

## �����������{@highlightTheme: ��������,(������ʱ�����ã����������С�)}

highlightTheme: default //TODO

## ���¹������ѹ��� {@warning:{days:�ٽ�����(Ĭ��300��,����0�رչ���),text:��������/*%dΪ����������ռλ��*/}}
warning:
  days: 300
  text: '������%d��֮ǰ�����������ݿ����Ѿ���ʱ��'

## ����������{@declaration: {enable:�Ƿ���,title:��������,tip:��ʾ����}}
declaration:
  enable: true
  title: 'ת������'
  tip: |-
      ��ҵת������ϵ���߻����Ȩ,����ҵת����ע������ ? <a href="" target="_blank">������</a>

## ���´���{@reward: {alipay:֧��������,wepay:΢�Ŵ���,tip:������ʾ��; ���Ӷ�Ϊ��,�رմ��͹���}}
reward:
  alipay: ''
  wepay: '../img/reward-wepay.jpg'
  tip: �����ǲ�ˣ��å�Ĺ���


## ��������

### gitment
gitment:
  enable: false
  owner:
  repo:
  client_id:
  client_secret:
  labels:
  perPage:
  maxCommentHeight:

### ������(Ĭ��ѡ��)
livere:
  enable: true
  livere_uid:

### ��������(�����ȶ��������޷�����)
uyan:
  enable: false
  uyan_id:

### Disqus����(��Ҫ��ǽ�����ߴ����)
disqus:
  enable: false
  shortname: snippet
  count: false

### ��������(��ҪICP����)
changyan:
  enable: false
  appid:
  conf:

### Valine���� �ο���վ: [valine����](https://valine.js.org/)
valine:
  enable: true
  appId:
  appKey:
  placeholder: ˵��ʲô��
  notify: false // �ʼ�֪ͨ
  verify: false // ��֤��
  avatar: mm // avatarͷ��
  meta: nick,mail // ��������ݣ���ѡֵnick,mail,link
  pageSize: 10

## ��վ�ÿ�ͳ�� [������ͳ��](http://busuanzi.ibruce.info/)
visit_counter:
   site: true // �ܷ������ͷ�������ͳ��
   page: true // �����Ķ���ͳ��

## ��վ����ͳ��

### ����CNZZͳ�� �ο���վ: [����CNZZ](http://www.umeng.com/)
cnzz_anaylytics:

### �ٶ�ͳ�� �ο���վ: [�ٶ�ͳ��](https://tongji.baidu.com/)
baidu_anaylytics:

### �ȸ�ͳ�� �ο���վ��[�ȸ�ͳ��](https://www.google-analytics.com/)
google_anaylytics:

### ��Ѷ���� �ο���վ��[��Ѷ����](http://ta.qq.com/)
tencent_analytics:

### �ٶ�վ����֤
baidu-site-verification:

### �ٶ��Զ�����(@baidu_push: �Ƿ����ðٶ��Զ�����)  �ο���վ: [�ٶ�վ����Դ](https://ziyuan.baidu.com/college/courseinfo?id=267&page=2#h2_article_title18)
baidu_push:

## ICON���� (���������ñ���Font Icon)
fontAwesome: //cdn.bootcss.com/font-awesome/4.7.0/css/font-awesome.min.css

## ��վ��������
since: 2017  //��վʱ��
robot: 'all'  //�������������ץȡ������������Ϊ��Ĭ��Ϊall
version: 1.2.1  //��ǰ����汾��
ʹ�ü��ɼ�������չ

1.�޸���������Front-matterģ��,�޸�scaffoldsĿ¼�µ�post.mdģ��

ģ���ļ��ڲ���Ҫ����ע�Ͳ���,�ؼ��ʺ�����ʹ��Ӣ��ð��
 ---
  title: {{ title }} // ����
  date: {{ date }}   // ʱ��
  categories: ['����1','����2'] // ����
  tags: ['��ǩ1','��ǩ2']       // ��ǩ
  comments: false    // �Ƿ�������
  img:               // �Զ�������ͼ
  ---
2.����վ�ڱ����������� ���Ҫʹ�ñ���վ�����������밲װ���hexo-generator-json-content��������������json�ļ�

npm i hexo-generator-json-content@2.2.0 -S
Ȼ���޸���������_config.yml�ļ���jsonContent��ز�����