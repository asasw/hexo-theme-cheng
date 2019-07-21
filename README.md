# Hexo-Theme
<a href="https://travis-ci.com/asasw/hexo-theme-cheng"><img src="https://travis-ci.com/asasw/hexo-theme-cheng.svg?branch=master" title="Travis CI"></a>
> [Kaijun](https://github.com/Kaijun/hexo-theme-huxblog) created this hexo theme and I modified it by consulting [huweihuang](https://github.com/huweihuang/hexo-theme-huweihuang) and [Liao can](https://github.com/nqmysb/hexo-theme-huweihuang). But this origin web theme created by [Hux Blog](http://huangxuan.me) using Jekyll. :blush:

### [View Live Cheng Blog &rarr;](https://cheng.cf)

![Theme_Cheng](https://upload.cc/i1/2019/07/19/uEWXKl.png)

# Install Hexo

First make sure you have installed 
- [Node.js](http://nodejs.org/)
- [Git](http://git-scm.com/)

If your computer already has these, just install Hexo with npm:

```bash
npm install -g hexo-cli
```

# Theme Usage

### Init

```bash
git clone https://github.com/asasw/hexo-theme-cheng.git 
cd hexo-theme-cheng
npm install
```

### Modify
Modify the `_config.yml` file with your own info. Especially the section:

##### Deployment
Replace to your own repo!
```yml
deploy:
  type: git
  repo: https://github.com/<yourAccount>/<repo>
  branch: <your-branch>
```

# Configuration

### Sidebar settings
Copy your avatar image to `cheng/source/img/` and modify the `theme _config.yml`:
```yml
sidebar: true    # whether or not using Sidebar.
sidebar-about-description: "<your description>"
sidebar-avatar: img/<your avatar path>
```
and activate your personal widget you like
```yml
widgets:         # here are widget you can use, you can comment out
- short-about
- featured-tags
- recent-posts
- archive
```
if you want to add sidebar widget, please add at `layout/_widget`.

### Go to top icon Setup
My icon is using rocket, you can change to your own icon at `cheng/source/img`.

### click_show_text
you can modify the content in `js/click_show_text.js`

### Analytics
Just checkout the code offered by Google/Baidu, and copy paste here, all the rest is already done for you.
```
# Google Analytics
ga_track_id: 'your track id'          # Format: UA-xxxxxx-xx
ga_domain: your domain  # cheng.cf
# Baidu Tongji
bd_track_id: your baidu track id
```
(Google might ask for meta tag "google-site-verification")

### Rewards
copy your alipay and wechatpay images to `cheng/source/img`, and change the filename.
```
reward: true
reward_comment: Give me a five
wechatpay: /img/wechat.jpg
alipay: /img/alipay.jpg
```

### Comment
I use the comment system - [Livere](https://www.livere.com/)
You could sign up the livere city version and copy the uid here
```
livere_uid: MTAyMC80NTE5Mi8yMTcwOA==
```

### Hexo Basics
Some hexo command:
```bash
hexo new "<post name>" # you can change post to another layout if you want
hexo c  # clean out the database and public/ files
hexo g # generate the static file
hexo s # run hexo in local environment
hexo d # hexo will push the static files automatically into the specific branch(gh-pages) of your repo!
```

# Support

- **Feel free to fork. I'll Appreciate it if you keep the Author & Github link at footer**
- Give it a **Star** if you like, fork or just clone to use 
- If any problem or requirement, just open an issue here and I will help you.
