# biographicalnotes<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=5.0, minimum-scale=0.1">
    <title>吴瑞鹏-简历</title>
    <style>
        :root {
            --primary-color: #2c3e50;
            --secondary-color: #3498db;
            --text-color: #34495e;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', 'PingFang SC', system-ui, sans-serif;
            line-height: 1.6;
            color: var(--text-color);
            background: #f8f9fa;
        }

        /* 容器系统 */
        .container {
            max-width: 1200px;
            width: 95%;
            margin: 0 auto;
            padding: 20px;
            overflow-x: hidden;
        }

        /* 头部样式 */
        header {
            text-align: center;
            padding: 2rem 1rem;
            background: linear-gradient(135deg, var(--primary-color), #4e5568);
            color: white;
            position: relative;
            margin-bottom: 2rem;
        }

        .avatar {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            margin: 1rem auto;
            border: 4px solid rgba(255,255,255,0.9);
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            object-fit: cover;
        }

        .avatar:hover {
            transform: rotate(5deg) scale(1.05);
            box-shadow: 0 8px 20px rgba(0,0,0,0.15);
        }

        /* 响应式网格系统 */
        .main-content {
            display: grid;
            grid-template-columns: 3fr 1fr;
            gap: 2rem;
            margin-top: 1rem;
        }

        /* 卡片组件 */
        .card {
            background: white;
            padding: 1.8rem;
            border-radius: 12px;
            box-shadow: 0 3px 6px rgba(0,0,0,0.1);
            margin-bottom: 1.5rem;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.15);
        }

        /* 技能标签系统 */
        .skill-tag {
            display: inline-block;
            padding: 8px 18px;
            background: var(--secondary-color);
            color: white;
            border-radius: 25px;
            margin: 6px;
            cursor: pointer;
            transition: all 0.2s;
            font-size: 0.9em;
        }

        .skill-tag:hover {
            background: #2980b9;
            transform: scale(1.05);
        }

        /* 时间轴组件 */
        .timeline {
            position: relative;
            padding-left: 30px;
            margin: 2rem 0;
        }

        .timeline::before {
            content: '';
            position: absolute;
            left: 6px;
            top: 0;
            height: 100%;
            width: 2px;
            background: var(--secondary-color);
        }

        .timeline-item {
            position: relative;
            margin-bottom: 2rem;
            padding-left: 25px;
        }

        .timeline-item::before {
            content: '';
            position: absolute;
            left: -6px;
            top: 8px;
            width: 14px;
            height: 14px;
            background: white;
            border: 3px solid var(--secondary-color);
            border-radius: 50%;
        }

       /* 打印按钮 */
       .print-btn {
            position: fixed;
            bottom: 20px;
            right: 20px;
            padding: 10px 20px;
            background: var(--primary-color);
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s;
        }

        .print-btn:hover {
            background: var(--secondary-color);
        }

        @media (max-width: 768px) {
            .main-content {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <header>
        <img src="C:\Users\昨日青空\OneDrive\图片\本机照片\7570cfa8eda3ae03.jpg" alt="个人头像" class="avatar">
        <h1>吴瑞鹏</h1>
        <p>项目经理 | 灵当高级实施工程师</p>
    </header>

    <div class="container">
        <div class="main-content">
            <main>
                <section class="card" id="profile">
                    <h2>📖 个人简介</h2>
                    <p>资深全栈工程师，6年互联网开发经验，主导过多个百万级用户项目。精通React生态和Node.js后端开发，熟悉微服务架构和DevOps实践。</p>
                </section>

                <section class="card" id="experience">
                    <h2>💼 工作经历</h2>
                    <div class="timeline">
                        <div class="timeline-item">
                            <h3>技术总监 - 创新科技</h3>
                            <p class="date">2021/03 - 至今</p>
                            <ul class="detail">
                                <li>主导技术团队管理（15人团队）</li>
                                <li>微服务架构设计与实施</li>
                                <li>研发效能提升方案落地</li>
                            </ul>
                        </div>
                        <div class="timeline-item">
                            <h3>高级开发工程师 - 云创科技</h3>
                            <p class="date">2018/06 - 2021/02</p>
                            <ul class="detail">
                                <li>核心业务系统重构</li>
                                <li>前端性能优化专项</li>
                                <li>Node.js中间件开发</li>
                            </ul>
                        </div>
                    </div>
                </section>
            </main>

            <aside>
                <section class="card" id="skills">
                    <h2>🛠 技术栈</h2>
                    <div class="skills-container"></div>
                </section>

                <section class="card" id="contact">
                    <h2>📱 联系方式</h2>
                    <ul>
                        <li>📧 lisi@dev.com</li>
                        <li>☎️ (+86) 138-1234-5678</li>
                        <li>📍 北京 · 海淀区</li>
                        <li>🌐 www.lisi-portfolio.com</li>
                    </ul>
                </section>
            </aside>
        </div>
    </div>

    <button class="print-btn" onclick="window.print()">🖨 打印简历</button>

    <script>
        // 动态技能标签生成
        const techStack = [
            'JavaScript (ES6+)', 'React 18', 'Node.js', 
            'TypeScript', 'Docker', 'Kubernetes',
            'AWS', 'GraphQL', 'MongoDB', 'Redis',
            'Webpack'
        ];

        const skillsContainer = document.querySelector('.skills-container');
        techStack.forEach(skill => {
            const tag = document.createElement('span');
            tag.className = 'skill-tag';
            tag.textContent = skill;
            tag.addEventListener('click', () => {
                const modal = document.createElement('div');
                modal.style.cssText = `
                    position: fixed;
                    top: 50%;
                    left: 50%;
                    transform: translate(-50%, -50%);
                    background: white;
                    padding: 20px;
                    border-radius: 8px;
                    box-shadow: 0 4px 12px rgba(0,0,0,0.2);
                    z-index: 1000;
                `;
                modal.innerHTML = `
                    <h3>${skill} 项目经验</h3>
                    <p>此处展示相关技术细节...{细节展示}</p>
                    <button onclick="this.parentElement.remove()">关闭</button>
                `;
                document.body.appendChild(modal);
            });
            skillsContainer.appendChild(tag);
        });

        // 卡片交互效果
        document.querySelectorAll('.card').forEach(card => {
            card.addEventListener('click', function() {
                this.classList.toggle('card-expanded');
            });
        });

        // 响应式检测
        function checkResponsive() {
            if (window.innerWidth <= 768) {
                document.body.classList.add('mobile-view');
            } else {
                document.body.classList.remove('mobile-view');
            }
        }
        window.addEventListener('resize', checkResponsive);
        checkResponsive();
    </script>
</body>
</html>
