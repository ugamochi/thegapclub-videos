# Push and Transfer Instructions

## Step 1: Create Repository on GitHub

1. Go to [github.com](https://github.com) and log in
2. Click "+" icon (top right) → "New repository"
3. Settings:
   - **Repository name**: `thegapclub-videos`
   - **Description**: "Video files for The Gap Club website"
   - **Public** ✅ (must be public)
   - **DO NOT** initialize with README (we already have one)
4. Click "Create repository"

## Step 2: Push to GitHub

Run these commands from the `thegapclub-videos` folder:

```bash
# Add your GitHub repo as remote (replace YOUR-USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR-USERNAME/thegapclub-videos.git

# Push to GitHub
git branch -M main
git push -u origin main
```

## Step 3: Verify URLs Work

Test these URLs in your browser (replace YOUR-USERNAME):

```
https://raw.githubusercontent.com/YOUR-USERNAME/thegapclub-videos/main/videos/custom-video.mp4
https://raw.githubusercontent.com/YOUR-USERNAME/thegapclub-videos/main/videos/testimonial-1.mp4
https://raw.githubusercontent.com/YOUR-USERNAME/thegapclub-videos/main/videos/testimonial-2.mp4
https://raw.githubusercontent.com/YOUR-USERNAME/thegapclub-videos/main/videos/testimonial-3.mp4
https://raw.githubusercontent.com/YOUR-USERNAME/thegapclub-videos/main/videos/testimonial-4.mp4
```

Videos should download or play.

## Step 4: Transfer to Client

Client info:
- **Username**: bemodo000
- **Email**: bemodo000@gmail.com

### Transfer Steps:

1. Go to your repository on GitHub: `https://github.com/YOUR-USERNAME/thegapclub-videos`
2. Click "Settings" tab
3. Scroll to bottom → "Danger Zone"
4. Click "Transfer ownership"
5. Enter: `bemodo000`
6. Type repository name to confirm: `thegapclub-videos`
7. Click "I understand, transfer this repository"

### Client Accepts Transfer:

Client will receive email from GitHub. They need to:
1. Click link in email
2. Click "Accept transfer"
3. Confirm

## Step 5: Update Webflow URLs

After transfer (or before, URLs will redirect), update Webflow:

### Custom Video Block
```html
<video 
  class="tgc-video" 
  src="https://raw.githubusercontent.com/bemodo000/thegapclub-videos/main/videos/custom-video.mp4"
  ...
```

### Testimonial Videos
```html
<div class="testim-video-container" 
     data-video-src="https://raw.githubusercontent.com/bemodo000/thegapclub-videos/main/videos/testimonial-1.mp4">

<div class="testim-video-container" 
     data-video-src="https://raw.githubusercontent.com/bemodo000/thegapclub-videos/main/videos/testimonial-2.mp4">

<div class="testim-video-container" 
     data-video-src="https://raw.githubusercontent.com/bemodo000/thegapclub-videos/main/videos/testimonial-3.mp4">

<div class="testim-video-container" 
     data-video-src="https://raw.githubusercontent.com/bemodo000/thegapclub-videos/main/videos/testimonial-4.mp4">
```

## Step 6: Test Everything

- [ ] Custom video loads and plays
- [ ] All 4 testimonial videos load and play
- [ ] Videos work on mobile
- [ ] No console errors

## Step 7: Send Client Confirmation

```
Привет,

Я перенес видео-репозиторий на ваш аккаунт GitHub.

Ваш репозиторий: https://github.com/bemodo000/thegapclub-videos

Что там:
• Все 5 видео для сайта
• Инструкции в README

Важно:
• Держите репозиторий публичным (Public)
• При обновлении видео используйте то же имя файла
• Если нужна помощь - пишите

Сайт теперь использует видео из вашего репозитория.
```

## Done!

Client now owns the repository and can manage videos independently.
