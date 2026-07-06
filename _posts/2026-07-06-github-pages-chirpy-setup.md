---
title: GitHub Pages와 Chirpy로 기술 블로그 만들기
date: 2026-07-06 00:00:00 +0900
categories: [Blog, GitHub Pages]
tags: [github-pages, jekyll, chirpy, blog]
description: GitHub Pages와 Jekyll Chirpy 테마를 이용해 기술 블로그를 만든 과정을 정리합니다.
---

# GitHub Pages와 Chirpy로 기술 블로그 만들기

기술 학습 내용과 프로젝트 기록을 정리하기 위해 GitHub Pages 기반의 블로그를 만들었다.

이번 글에서는 블로그를 만들면서 진행한 과정을 정리한다.

## 사용한 도구

- GitHub Pages
- Jekyll
- Chirpy Theme
- GitHub Actions

## 진행 과정

### 1. Chirpy Starter 저장소 생성

처음에는 빈 `wonnie219.github.io` 저장소를 만들었지만, Chirpy 테마 파일이 들어있지 않아 `_config.yml`, `_posts`, `_tabs` 폴더가 없었다.

그래서 `cotes2020/chirpy-starter` 템플릿을 사용해 다시 저장소를 생성했다.

### 2. GitHub Pages 설정

저장소의 `Settings → Pages`에서 배포 방식을 `GitHub Actions`로 설정했다.

이 설정을 통해 Markdown 글과 Chirpy 테마가 GitHub Actions에서 빌드되고, 완성된 HTML 사이트가 GitHub Pages로 배포된다.

### 3. 기본 설정 수정

`_config.yml` 파일에서 블로그 제목, 설명, 언어, 시간대를 수정했다.

```yml
lang: ko-KR
timezone: Asia/Seoul
url: "https://wonnie219.github.io"
