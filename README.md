 <!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
    <title>培智学生职业教育学习效果评价工具表｜层级合并版｜含等级描述</title>
    <style>
        * {
            box-sizing: border-box;
        }
        body {
            background: #eef2f7;
            font-family: 'Segoe UI', Roboto, 'Noto Sans', system-ui, -apple-system, 'Helvetica Neue', sans-serif;
            margin: 0;
            padding: 20px 16px;
            color: #1a2c3e;
        }
        .container {
            max-width: 1600px;
            margin: 0 auto;
            background: white;
            border-radius: 28px;
            box-shadow: 0 12px 30px rgba(0,0,0,0.08);
            overflow-x: auto;
            padding: 20px 20px 32px;
        }
        h1 {
            font-size: 1.8rem;
            font-weight: 700;
            margin-top: 0;
            margin-bottom: 0.2rem;
            color: #0b3954;
            border-left: 6px solid #2c7da0;
            padding-left: 18px;
        }
        .sub {
            color: #2c6979;
            margin-bottom: 20px;
            font-size: 0.9rem;
            border-bottom: 1px solid #d4dee5;
            padding-bottom: 10px;
            margin-top: 6px;
            padding-left: 24px;
        }
        .info-panel {
            background: #f8fafc;
            border-radius: 20px;
            padding: 16px 20px;
            margin-bottom: 25px;
            display: flex;
            flex-wrap: wrap;
            gap: 18px;
            border: 1px solid #e2edf2;
        }
        .info-field {
            flex: 1;
            min-width: 150px;
        }
        .info-field label {
            display: block;
            font-weight: 600;
            font-size: 0.75rem;
            color: #2c7da0;
            letter-spacing: 0.5px;
            margin-bottom: 6px;
        }
        .info-field input, .info-field select {
            width: 100%;
            padding: 8px 12px;
            border-radius: 20px;
            border: 1px solid #cbdde6;
            background: white;
            font-size: 0.85rem;
        }
        .score-summary {
            background: #e6f4f1;
            border-radius: 24px;
            padding: 14px 24px;
            margin-bottom: 24px;
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            align-items: center;
            gap: 16px;
        }
        .total-box {
            background: #0b3954;
            color: white;
            padding: 10px 24px;
            border-radius: 48px;
            font-weight: 700;
            font-size: 1.7rem;
            min-width: 190px;
            text-align: center;
        }
        .total-box span {
            font-size: 0.8rem;
            font-weight: normal;
            display: block;
            margin-top: 4px;
        }
        .level-badge {
            background: white;
            border-radius: 40px;
            padding: 6px 24px;
            font-weight: 600;
            color: #1e5a6e;
            border-left: 5px solid #2c7da0;
        }
        .action-buttons {
            display: flex;
            gap: 12px;
        }
        button {
            background: #2c7da0;
            border: none;
            color: white;
            font-weight: 600;
            padding: 8px 20px;
            border-radius: 40px;
            cursor: pointer;
            font-size: 0.8rem;
            transition: 0.2s;
        }
        button:hover {
            background: #1f5e7a;
            transform: translateY(-1px);
        }
        button.reset-btn {
            background: #94a3b8;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            font-size: 0.8rem;
            box-shadow: 0 1px 2px rgba(0,0,0,0.03);
            min-width: 1100px;
            border-radius: 20px;
            overflow: hidden;
        }
        th {
            background: #eef2f9;
            color: #1e3a4d;
            padding: 12px 8px;
            font-weight: 700;
            border: 1px solid #cfdfe8;
            font-size: 0.82rem;
        }
        td {
            border: 1px solid #e2edf2;
            padding: 10px 8px;
            vertical-align: top;
            background-color: white;
        }
        .level1-cell, .level2-cell {
            background-color: #f9fbfd;
            font-weight: 600;
            vertical-align: middle;
        }
        .level1-cell {
            background-color: #f0f5fa;
            font-weight: 700;
        }
        .desc-cell {
            font-weight: 500;
        }
        .weight-cell {
            text-align: center;
            font-weight: 600;
            background: #f9f9fe;
            width: 55px;
        }
        .score-cell {
            text-align: center;
            width: 95px;
        }
        select {
            padding: 6px 4px;
            border-radius: 26px;
            border: 1px solid #bcd3df;
            background: white;
            font-weight: 500;
            width: 85px;
            cursor: pointer;
            font-size: 0.75rem;
        }
        .actual-score {
            font-weight: 700;
            color: #1e6f5c;
            background: #f0f9f6;
            border-radius: 40px;
            display: inline-block;
            padding: 4px 10px;
            min-width: 55px;
            text-align: center;
            font-size: 0.8rem;
        }
        .level-desc-cell {
            font-size: 0.7rem;
            line-height: 1.45;
            color: #2c5a6e;
            background: #fefcf5;
            min-width: 250px;
            word-break: break-word;
        }
        .level-desc-cell strong {
            color: #0f5c6b;
        }
        .text-center {
            text-align: center;
        }
        .footer-note {
            margin-top: 28px;
            background: #f7fafc;
            padding: 16px 20px;
            border-radius: 24px;
            font-size: 0.75rem;
            color: #2c6075;
        }
        @media (max-width: 1200px) {
            .level-desc-cell {
                font-size: 0.65rem;
            }
        }
    </style>
</head>
<body>
<div class="container">
    <h1>📊 培智学生职业教育学习效果评价工具表</h1>
    <div class="sub">基于德尔菲权重体系 · 一级/二级指标合并展示（层级清晰） · 每个条目附带1~5级具体行为标准</div>

    <!-- 学生信息栏 -->
    <div class="info-panel">
        <div class="info-field"><label>👤 学生姓名</label><input type="text" id="studentName" placeholder="例：张明"></div>
        <div class="info-field"><label>⚥ 性别</label><select id="gender"><option>男</option><option>女</option></select></div>
        <div class="info-field"><label>📅 年龄</label><input type="text" id="age" placeholder="岁"></div>
        <div class="info-field"><label>🏫 班级/年级</label><input type="text" id="classGrade" placeholder="职教班"></div>
        <div class="info-field"><label>📝 评价人</label><select id="evaluator"><option>班主任</option><option>职业课教师</option><option>家长</option><option>其他</option></select></div>
        <div class="info-field"><label>📅 评价日期</label><input type="date" id="evalDate" value="2026-05-22"></div>
    </div>

    <div class="score-summary">
        <div class="total-box" id="totalScoreBox">0.00 <span>综合得分 (满分100)</span></div>
        <div class="level-badge" id="levelDesc">未评分</div>
        <div class="action-buttons">
            <button id="resetAllBtn" class="reset-btn">🔄 重置所有评分为3分(一般)</button>
            <button id="exportBtn">📋 复制结果摘要</button>
        </div>
    </div>

    <div style="overflow-x: auto;">
        <table id="evaluationTable">
            <thead>
                <tr>
                    <th style="width:12%">一级指标</th>
                    <th style="width:14%">二级指标</th>
                    <th style="width:22%">三级指标（评价条目）</th>
                    <th style="width:6%">满分</th>
                    <th style="width:10%">等级评分(1-5)</th>
                    <th style="width:8%">实际得分</th>
                    <th style="width:28%">📌 各等级具体要求(1分～5分)</th>
                </tr>
            </thead>
            <tbody id="tableBody">
                <!-- 动态生成，支持行合并 -->
            </tbody>
        </table>
    </div>

    <div class="footer-note">
        <strong>📌 评价指引：</strong> 每个三级指标均附有1~5分的具体行为描述，请根据学生近期真实表现选择最适合的等级。系统将根据权重自动计算加权得分。<br>
        <strong>等级意义：</strong> 5分=完全达到/独立稳定完成；4分=较好达到/少量辅助；3分=基本达到/部分提示；2分=较差/较多支持；1分=未达标/完全依赖。<br>
        <strong>总分参考：</strong> ≥90优秀，75-89良好，60-74中等，40-59待提高，&lt;40需重点干预。
    </div>
</div>

<script>
    // ==================== 指标体系（含权重）====================
    // 依据原始权重表, 62个三级指标, 总分100
    const indicatorsRaw = [
        // A1 职业认知 (10分)
        { level1: "A1 职业认知", level2: "B1.1 岗位认知", desc: "C1.1.1 了解工作内容", weight: 1.5 },
        { level1: "A1 职业认知", level2: "B1.1 岗位认知", desc: "C1.1.2 了解工作环境", weight: 1.0 },
        { level1: "A1 职业认知", level2: "B1.1 岗位认知", desc: "C1.1.3 了解岗位要求", weight: 1.5 },
        { level1: "A1 职业认知", level2: "B1.2 就业方向认知", desc: "C1.2.1 了解就业方向", weight: 3.0 },
        { level1: "A1 职业认知", level2: "B1.3 价值认知", desc: "C1.3.1 了解职业社会价值", weight: 3.0 },
        
        // A2 职业能力 (30分)
        { level1: "A2 职业能力", level2: "B2.1 职业知识", desc: "C2.1.1 专业基础知识", weight: 2.0 },
        { level1: "A2 职业能力", level2: "B2.1 职业知识", desc: "C2.1.2 工具设备识别", weight: 1.5 },
        { level1: "A2 职业能力", level2: "B2.1 职业知识", desc: "C2.1.3 操作流程知识", weight: 2.0 },
        { level1: "A2 职业能力", level2: "B2.1 职业知识", desc: "C2.1.4 安全规范常识", weight: 1.5 },
        { level1: "A2 职业能力", level2: "B2.1 职业知识", desc: "C2.1.5 劳动权益常识", weight: 1.0 },
        { level1: "A2 职业能力", level2: "B2.2 操作技能", desc: "C2.2.1 操作独立性", weight: 2.5 },
        { level1: "A2 职业能力", level2: "B2.2 操作技能", desc: "C2.2.2 操作规范性", weight: 2.0 },
        { level1: "A2 职业能力", level2: "B2.2 操作技能", desc: "C2.2.3 操作准确性", weight: 2.0 },
        { level1: "A2 职业能力", level2: "B2.2 操作技能", desc: "C2.2.4 操作连贯性", weight: 1.5 },
        { level1: "A2 职业能力", level2: "B2.2 操作技能", desc: "C2.2.5 操作完整性", weight: 1.5 },
        { level1: "A2 职业能力", level2: "B2.2 操作技能", desc: "C2.2.6 操作时效性", weight: 1.5 },
        { level1: "A2 职业能力", level2: "B2.2 操作技能", desc: "C2.2.7 成果达标度", weight: 1.5 },
        { level1: "A2 职业能力", level2: "B2.2 操作技能", desc: "C2.2.8 问题解决能力", weight: 1.5 },
        { level1: "A2 职业能力", level2: "B2.3 能力纵向发展", desc: "C2.3.1 知识技能提升度", weight: 2.0 },
        { level1: "A2 职业能力", level2: "B2.3 能力纵向发展", desc: "C2.3.2 操作熟练提升度", weight: 2.0 },
        { level1: "A2 职业能力", level2: "B2.3 能力纵向发展", desc: "C2.3.3 策略运用能力", weight: 1.5 },
        { level1: "A2 职业能力", level2: "B2.3 能力纵向发展", desc: "C2.3.4 抗挫能力提升度", weight: 1.5 },
        { level1: "A2 职业能力", level2: "B2.3 能力纵向发展", desc: "C2.3.5 自信心提升度", weight: 1.0 },
        
        // A3 职业素养 (25分)
        { level1: "A3 职业素养", level2: "B3.1 职业态度", desc: "C3.1.1 职业认同度", weight: 1.0 },
        { level1: "A3 职业素养", level2: "B3.1 职业态度", desc: "C3.1.2 职业偏好度", weight: 0.5 },
        { level1: "A3 职业素养", level2: "B3.1 职业态度", desc: "C3.1.3 职业学习主动性", weight: 1.5 },
        { level1: "A3 职业素养", level2: "B3.1 职业态度", desc: "C3.1.4 职业学习坚持性", weight: 1.5 },
        { level1: "A3 职业素养", level2: "B3.1 职业态度", desc: "C3.1.5 自我效能感", weight: 1.0 },
        { level1: "A3 职业素养", level2: "B3.1 职业态度", desc: "C3.1.6 接受指正态度", weight: 1.0 },
        { level1: "A3 职业素养", level2: "B3.1 职业态度", desc: "C3.1.7 服从指令意识", weight: 0.5 },
        { level1: "A3 职业素养", level2: "B3.2 工作品质", desc: "C3.2.1 对任务认真负责", weight: 2.0 },
        { level1: "A3 职业素养", level2: "B3.2 工作品质", desc: "C3.2.2 节约物料，爱护工具", weight: 1.5 },
        { level1: "A3 职业素养", level2: "B3.2 工作品质", desc: "C3.2.3 适应岗位体力要求", weight: 1.5 },
        { level1: "A3 职业素养", level2: "B3.2 工作品质", desc: "C3.2.4 面对困难时情绪稳定", weight: 1.0 },
        { level1: "A3 职业素养", level2: "B3.3 规范遵守", desc: "C3.3.1 遵守工作规章制度", weight: 2.0 },
        { level1: "A3 职业素养", level2: "B3.3 规范遵守", desc: "C3.3.2 保持工位整洁", weight: 1.5 },
        { level1: "A3 职业素养", level2: "B3.3 规范遵守", desc: "C3.3.3 保持个人卫生", weight: 1.5 },
        { level1: "A3 职业素养", level2: "B3.4 人际沟通", desc: "C3.4.1 准确理解工作指令", weight: 1.0 },
        { level1: "A3 职业素养", level2: "B3.4 人际沟通", desc: "C3.4.2 合理表达自身需求", weight: 1.0 },
        { level1: "A3 职业素养", level2: "B3.4 人际沟通", desc: "C3.4.3 使用礼貌用语", weight: 0.5 },
        { level1: "A3 职业素养", level2: "B3.4 人际沟通", desc: "C3.4.4 清晰传递工作信息", weight: 0.5 },
        { level1: "A3 职业素养", level2: "B3.4 人际沟通", desc: "C3.4.5 接受他人帮助", weight: 0.5 },
        { level1: "A3 职业素养", level2: "B3.4 人际沟通", desc: "C3.4.6 配合他人完成任务", weight: 1.0 },
        { level1: "A3 职业素养", level2: "B3.4 人际沟通", desc: "C3.4.7 主动帮助同伴", weight: 1.0 },
        { level1: "A3 职业素养", level2: "B3.4 人际沟通", desc: "C3.4.8 妥善化解人际矛盾", weight: 1.0 },
        { level1: "A3 职业素养", level2: "B3.4 人际沟通", desc: "C3.4.9 遇到危险时寻求帮助", weight: 0.5 },
        
        // A4 就业准备 (15分)
        { level1: "A4 就业准备", level2: "B4.1 求职准备", desc: "C4.1.1 了解求职基本流程", weight: 2.0 },
        { level1: "A4 就业准备", level2: "B4.1 求职准备", desc: "C4.1.2 了解招工信息获取途径", weight: 2.0 },
        { level1: "A4 就业准备", level2: "B4.1 求职准备", desc: "C4.1.3 主动询问或寻找就业机会", weight: 1.5 },
        { level1: "A4 就业准备", level2: "B4.1 求职准备", desc: "C4.1.4 积极参与实习或试岗", weight: 1.5 },
        { level1: "A4 就业准备", level2: "B4.2 岗位适应", desc: "C4.2.1 在真实或模拟环境中完成岗位任务", weight: 2.5 },
        { level1: "A4 就业准备", level2: "B4.2 岗位适应", desc: "C4.2.2 逐步适应职场的作息与工作强度", weight: 2.0 },
        { level1: "A4 就业准备", level2: "B4.2 岗位适应", desc: "C4.2.3 能说出自己做得好的和需要改进的地方", weight: 1.5 },
        { level1: "A4 就业准备", level2: "B4.2 岗位适应", desc: "C4.2.4 在多个可选岗位中做出适合自己的选择", weight: 2.0 },
        
        // A5 技能生活化应用 (20分)
        { level1: "A5 技能生活化应用", level2: "B5.1 生活场景迁移", desc: "C5.1.1 将所学技能应用于家庭场景", weight: 4.0 },
        { level1: "A5 技能生活化应用", level2: "B5.1 生活场景迁移", desc: "C5.1.2 在非训练环境中保持操作规范", weight: 3.0 },
        { level1: "A5 技能生活化应用", level2: "B5.1 生活场景迁移", desc: "C5.1.3 面对场景变化时能灵活调整", weight: 3.0 },
        { level1: "A5 技能生活化应用", level2: "B5.2 生活品质改善", desc: "C5.2.1 独立完成生活事务的质量提升", weight: 2.5 },
        { level1: "A5 技能生活化应用", level2: "B5.2 生活品质改善", desc: "C5.2.2 主动运用技能解决生活问题", weight: 2.5 },
        { level1: "A5 技能生活化应用", level2: "B5.2 生活品质改善", desc: "C5.2.3 记录和管理个人劳动报酬", weight: 2.0 },
        { level1: "A5 技能生活化应用", level2: "B5.2 生活品质改善", desc: "C5.2.4 合理规划劳动报酬的用途", weight: 1.5 },
        { level1: "A5 技能生活化应用", level2: "B5.2 生活品质改善", desc: "C5.2.5 参与家庭活动的程度提高", weight: 1.5 }
    ];
    
    // 智能生成每个指标的五级具体描述（详细）
    function generateLevelDescription(keyword, fullDesc) {
        // 根据具体指标名称定制精细描述，使评价更具针对性
        if (fullDesc.includes("独立性")) return "5分：完全独立完成全部操作，无需任何提醒或辅助；4分：基本独立，偶尔语言提示即可；3分：需要少量肢体示范或部分支持；2分：需要较多协助才能完成操作；1分：完全依赖他人，无法独立任何环节。";
        if (fullDesc.includes("规范性")) return "5分：操作全程符合标准流程，无任何违规；4分：大部分符合规范，极少偏差；3分：基本符合，部分步骤需纠正；2分：操作随意，多数环节不规范；1分：完全不符合规范要求。";
        if (fullDesc.includes("准确性")) return "5分：操作准确无误，成果正确率≥95%；4分：极少错误，准确率85%-94%；3分：主要步骤正确，准确率70%-84%；2分：错误较多，准确率<50%；1分：几乎全部错误。";
        if (fullDesc.includes("连贯") || fullDesc.includes("流畅")) return "5分：动作行云流水，无中断无停滞；4分：动作基本连贯，偶有短暂停顿；3分：有明显停顿但可自行继续；2分：频繁中断需提醒；1分：完全不能形成连贯动作。";
        if (fullDesc.includes("时效") || fullDesc.includes("时间")) return "5分：在规定时间内高效超额完成；4分：按时完成，质量较好；3分：略微超时但完成任务；2分：严重超时或仅完成少量；1分：无法按时完成任何部分。";
        if (fullDesc.includes("主动") || fullDesc.includes("积极性")) return "5分：非常主动，自发启动学习或任务；4分：较主动，偶尔激励即可；3分：被动参与，需明确指令；2分：极少主动，反复督促；1分：完全拒绝或逃避。";
        if (fullDesc.includes("坚持")) return "5分：遇到困难从不放弃，坚持完成；4分：多数情况能坚持；3分：有时放弃，经鼓励可继续；2分：经常半途而废；1分：完全不能坚持。";
        if (fullDesc.includes("情绪稳定") || fullDesc.includes("抗挫")) return "5分：挫折面前始终情绪平稳；4分：偶尔激动但快速平复；3分：有明显情绪波动但能调控；2分：情绪易失控影响任务；1分：完全无法控制情绪。";
        if (fullDesc.includes("理解指令")) return "5分：立即准确理解并执行复杂指令；4分：能理解大部分指令；3分：理解简单或常规指令；2分：仅理解极个别指令；1分：完全不能理解工作指令。";
        if (fullDesc.includes("表达需求")) return "5分：清晰主动表达自身需求；4分：基本能表达意愿；3分：提示下可表达；2分：极少主动表达；1分：完全不能表达。";
        if (fullDesc.includes("礼貌")) return "5分：主动且恰当使用礼貌用语；4分：偶尔忘记但能提醒后使用；3分：提示下使用礼貌用语；2分：基本不会使用；1分：拒绝使用礼貌用语。";
        if (fullDesc.includes("求职") || fullDesc.includes("就业机会") || fullDesc.includes("实习")) return "5分：完全掌握求职流程并积极行动；4分：较好了解，主动参与；3分：基本了解，需他人推动；2分：了解很少，被动；1分：完全不了解/不行动。";
        if (fullDesc.includes("报酬") || fullDesc.includes("规划") && fullDesc.includes("管理")) return "5分：独立管理报酬并能合理规划用途；4分：能管理但规划需指导；3分：在协助下管理；2分：依赖他人管理；1分：完全无意识。";
        if (fullDesc.includes("迁移") || fullDesc.includes("应用") || fullDesc.includes("家庭场景") || fullDesc.includes("生活")) {
            if (fullDesc.includes("家庭")) return "5分：熟练将技能迁移至家庭，独立应用且质量高；4分：较好应用，偶需提醒；3分：部分应用，效果一般；2分：极少应用，大量辅助；1分：无法迁移。";
            return "5分：完全能够将职业能力迁移到生活中，表现稳定；4分：较好迁移，偶尔不足；3分：基本能应用；2分：部分应用或需支持；1分：不能迁移。";
        }
        // 通用精细化描述
        return "5分：完全达成目标，表现卓越，独立稳定；4分：较好达成，偶尔需少量支持；3分：基本达成，需部分提示或辅助；2分：部分达成，需要大量支持；1分：无法达成，完全依赖。";
    }
    
    // 根据数据构建合并行信息
    function buildMergedTableData() {
        const rows = [];
        let lastLevel1 = "";
        let lastLevel2 = "";
        for (let item of indicatorsRaw) {
            const isNewLevel1 = (item.level1 !== lastLevel1);
            const isNewLevel2 = (item.level1 !== lastLevel1) || (item.level2 !== lastLevel2);
            const levelDescText = generateLevelDescription(item.desc, item.desc);
            rows.push({
                level1: item.level1,
                level2: item.level2,
                desc: item.desc,
                weight: item.weight,
                showLevel1: isNewLevel1,
                showLevel2: isNewLevel2,
                levelDesc: levelDescText
            });
            lastLevel1 = item.level1;
            lastLevel2 = item.level2;
        }
        // 计算每个一级指标跨行数 & 二级指标跨行数 (用于rowspan)
        const level1Spans = {};
        const level2Spans = {};
        for (let item of indicatorsRaw) {
            level1Spans[item.level1] = (level1Spans[item.level1] || 0) + 1;
            const key2 = `${item.level1}|${item.level2}`;
            level2Spans[key2] = (level2Spans[key2] || 0) + 1;
        }
        return { rows, level1Spans, level2Spans };
    }
    
    let rowComponents = []; // 存储每行的 { selectEl, scoreSpan, weight }
    
    function renderMergedTable() {
        const { rows, level1Spans, level2Spans } = buildMergedTableData();
        const tbody = document.getElementById('tableBody');
        tbody.innerHTML = '';
        rowComponents = [];
        
        for (let i = 0; i < rows.length; i++) {
            const r = rows[i];
            const tr = document.createElement('tr');
            // 一级指标
            const tdL1 = document.createElement('td');
            if (r.showLevel1) {
                tdL1.textContent = r.level1;
                const rowspan = level1Spans[r.level1];
                if (rowspan > 1) tdL1.rowSpan = rowspan;
                tdL1.className = "level1-cell";
                tdL1.style.backgroundColor = "#eef3fc";
                tdL1.style.fontWeight = "bold";
            } else {
                tdL1.style.display = "none";
            }
            // 二级指标
            const tdL2 = document.createElement('td');
            const l2key = `${r.level1}|${r.level2}`;
            if (r.showLevel2) {
                tdL2.textContent = r.level2;
                const rowspan = level2Spans[l2key];
                if (rowspan > 1) tdL2.rowSpan = rowspan;
                tdL2.className = "level2-cell";
                tdL2.style.backgroundColor = "#f7fafc";
            } else {
                tdL2.style.display = "none";
            }
            // 三级指标描述
            const tdDesc = document.createElement('td');
            tdDesc.textContent = r.desc;
            tdDesc.classList.add('desc-cell');
            // 权重值
            const tdWeight = document.createElement('td');
            tdWeight.textContent = r.weight.toFixed(1);
            tdWeight.classList.add('weight-cell', 'text-center');
            // 评分下拉
            const tdSelect = document.createElement('td');
            tdSelect.classList.add('score-cell');
            const select = document.createElement('select');
            for (let v = 1; v <= 5; v++) {
                const opt = document.createElement('option');
                opt.value = v;
                let label = '';
                if (v === 5) label = '5分-优秀';
                else if (v === 4) label = '4分-良好';
                else if (v === 3) label = '3分-一般';
                else if (v === 2) label = '2分-较差';
                else label = '1分-很差';
                opt.textContent = label;
                if (v === 3) opt.selected = true;
                select.appendChild(opt);
            }
            tdSelect.appendChild(select);
            // 实际得分显示
            const tdActual = document.createElement('td');
            tdActual.classList.add('score-cell');
            const actualSpan = document.createElement('span');
            actualSpan.classList.add('actual-score');
            actualSpan.textContent = '0.00';
            tdActual.appendChild(actualSpan);
            // 等级描述
            const tdLevelDesc = document.createElement('td');
            tdLevelDesc.classList.add('level-desc-cell');
            tdLevelDesc.innerHTML = `<strong>📋 等级要求</strong><br>${r.levelDesc}`;
            
            // 按需添加单元格 (保持顺序)
            if (r.showLevel1) tr.appendChild(tdL1);
            else tr.appendChild(document.createElement('td')); // 占位但隐藏样式
            if (r.showLevel2) tr.appendChild(tdL2);
            else tr.appendChild(document.createElement('td'));
            tr.appendChild(tdDesc);
            tr.appendChild(tdWeight);
            tr.appendChild(tdSelect);
            tr.appendChild(tdActual);
            tr.appendChild(tdLevelDesc);
            
            // 对于隐藏的占位单元格也要设置不可见
            if (!r.showLevel1) tr.children[0].style.display = 'none';
            if (!r.showLevel2) tr.children[1].style.display = 'none';
            
            tbody.appendChild(tr);
            
            rowComponents.push({
                selectEl: select,
                scoreSpan: actualSpan,
                weight: r.weight
            });
            updateSingleRowComponent(rowComponents[rowComponents.length-1]);
        }
        
        // 绑定事件与初始总分
        rowComponents.forEach(ref => {
            ref.selectEl.addEventListener('change', () => {
                updateSingleRowComponent(ref);
                updateTotalScoreComputed();
            });
        });
        updateTotalScoreComputed();
    }
    
    function updateSingleRowComponent(ref) {
        const rank = parseInt(ref.selectEl.value, 10);
        const actual = (ref.weight * rank) / 5;
        ref.scoreSpan.textContent = actual.toFixed(2);
    }
    
    function updateTotalScoreComputed() {
        let total = 0;
        rowComponents.forEach(ref => {
            const rank = parseInt(ref.selectEl.value, 10);
            total += (ref.weight * rank) / 5;
        });
        const totalFixed = total.toFixed(2);
        document.getElementById('totalScoreBox').innerHTML = `${totalFixed} <span>综合得分 (满分100)</span>`;
        let levelText = '';
        if (total >= 90) levelText = '🌟 优秀 (90-100)';
        else if (total >= 75) levelText = '✅ 良好 (75-89)';
        else if (total >= 60) levelText = '📘 中等 (60-74)';
        else if (total >= 40) levelText = '⚠️ 待提高 (40-59)';
        else levelText = '❗ 需重点干预 (<40)';
        document.getElementById('levelDesc').innerHTML = `等级参考: ${levelText}`;
        return total;
    }
    
    function resetAllToThree() {
        rowComponents.forEach(ref => {
            ref.selectEl.value = '3';
            updateSingleRowComponent(ref);
        });
        updateTotalScoreComputed();
    }
    
    function exportSummary() {
        const student = document.getElementById('studentName').value || '未填写';
        const gender = document.getElementById('gender').value;
        const age = document.getElementById('age').value || '—';
        const classInfo = document.getElementById('classGrade').value || '—';
        const evaluator = document.getElementById('evaluator').value;
        const evalDate = document.getElementById('evalDate').value;
        const totalScore = document.getElementById('totalScoreBox').innerText.split(' ')[0];
        const levelDescRaw = document.getElementById('levelDesc').innerText;
        let summary = `【培智学生职业教育学习效果评价摘要】\n学生：${student} | 性别：${gender} | 年龄：${age}\n班级：${classInfo} | 评价人：${evaluator} | 日期：${evalDate}\n━━━━━━━━━━━━━━━━━━━━━━━━\n📊 综合总分：${totalScore} / 100\n🏆 ${levelDescRaw}\n📌 评价条目总数：${rowComponents.length}项 (每项均含具体等级描述)\n说明：各条目等级详细要求已在表格中展示。`;
        navigator.clipboard.writeText(summary).then(() => alert("✅ 评价摘要已复制到剪贴板")).catch(() => prompt("手动复制", summary));
    }
    
    window.onload = () => {
        renderMergedTable();
        document.getElementById('resetAllBtn').addEventListener('click', resetAllToThree);
        document.getElementById('exportBtn').addEventListener('click', exportSummary);
        if(!document.getElementById('evalDate').value) {
            document.getElementById('evalDate').value = new Date().toISOString().slice(0,10);
        }
    };
</script>
</body>
</html>
