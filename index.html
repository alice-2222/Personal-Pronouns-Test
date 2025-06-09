# Personal-Pronouns-Test
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Advanced Personal Pronouns Grammar Quiz</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            padding: 20px;
            background: #f2f2f2;
            max-width: 800px;
            margin: 0 auto;
        }
        .question {
            background: #fff;
            padding: 15px;
            margin-bottom: 10px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        .result {
            background: #e6ffe6;
            padding: 20px;
            border-radius: 8px;
            margin-top: 20px;
        }
        button {
            background-color: #4CAF50;
            color: white;
            padding: 12px 20px;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            font-size: 16px;
            margin-right: 10px;
        }
        button:hover {
            background-color: #45a049;
        }
        .history {
            background: #e6f3ff;
            padding: 20px;
            border-radius: 8px;
            margin-top: 20px;
        }
        .hidden {
            display: none;
        }
        .tabs {
            display: flex;
            margin-bottom: 20px;
        }
        .tab {
            padding: 10px 20px;
            background: #ddd;
            cursor: pointer;
            border-radius: 5px 5px 0 0;
            margin-right: 5px;
        }
        .tab.active {
            background: #4CAF50;
            color: white;
        }
        .tab-content {
            display: none;
        }
        .tab-content.active {
            display: block;
        }
        .correct {
            color: green;
        }
        .incorrect {
            color: red;
        }
        .save-buttons {
            margin-top: 20px;
            text-align: center;
        }
        .save-btn {
            background-color: #2196F3;
            margin: 5px;
        }
        .save-btn:hover {
            background-color: #0b7dda;
        }
    </style>
</head>
<body>

<h2>Advanced Personal Pronouns Grammar Quiz</h2>

<div class="tabs">
    <div class="tab active" onclick="showTab('quiz')">做测验</div>
    <div class="tab" onclick="showTab('history')">查看记录</div>
</div>

<div id="quiz" class="tab-content active">
    <form id="quizForm">
        <label>Name (名字):</label><br>
        <input type="text" id="name" required><br><br>

        <label>Form (年级):</label><br>
        <input type="text" id="form" required><br><br>

        <div id="questions"></div>

        <button type="button" onclick="submitQuiz()">提交答案</button>
        <button type="button" onclick="saveProgress()">保存进度</button>
        <button type="button" onclick="loadProgress()">加载进度</button>
    </form>

    <div id="result" class="result hidden"></div>
</div>

<div id="history" class="tab-content">
    <h3>你的测验记录</h3>
    <div id="historyList"></div>
</div>

<script>
const questions = [
    {
        q: "Neither John nor ___ could answer the question.",
        options: ["I", "me", "myself", "mine"],
        answer: "I",
        explain: "这里要用'I'，因为说的是'John不能回答，我也不能回答'，就像说'I could not answer'一样。",
        encourage: "这个句型确实有点绕，不过你能尝试就很棒啦！记住：'neither A nor B'后面要跟着平时说话时的样子哦~"
    },
    {
        q: "Between you and ___, I think we should reconsider.",
        options: ["I", "me", "myself", "mine"],
        answer: "me",
        explain: "这里用'me'就对了，就像平时说'between us'一样自然。",
        encourage: "介词后面的词确实容易搞混呢！不过没关系，多练习几次就会记住啦！"
    },
    {
        q: "It was ___ who solved the problem.",
        options: ["he", "him", "his", "himself"],
        answer: "he",
        explain: "这里强调'是他解决了问题'，所以要用'he'，就像平时说'He solved it'一样。",
        encourage: "强调句确实需要多想想呢！你的思考方向是对的，下次一定会更准确！"
    },
    {
        q: "The teacher gave Sarah and ___ extra homework.",
        options: ["I", "me", "myself", "mine"],
        answer: "me",
        explain: "这里要用'me'，因为是老师给'我'作业，就像说'gave me'一样。",
        encourage: "双宾语结构不容易，但你已经很接近答案啦！记住：动词后面通常用'me'这样的形式~"
    },
    {
        q: "___ and your brother need to finish the project.",
        options: ["You", "Your", "Yours", "Yourself"],
        answer: "You",
        explain: "这里用'You'开头，因为是'你和你的兄弟'需要完成项目，就像说'You need'一样。",
        encourage: "并列主语的选择很重要，你已经理解了基本概念！真棒！"
    },
    {
        q: "The decision is up to ___.",
        options: ["she", "her", "hers", "herself"],
        answer: "her",
        explain: "这里用'her'，就像平时说'up to me'一样，介词后面用这个形式。",
        encourage: "短语后的代词形式容易错，但你的直觉很准！再多练习几次就熟练啦！"
    },
    {
        q: "No one but ___ knew the secret.",
        options: ["he", "him", "his", "himself"],
        answer: "him",
        explain: "这里的'but'相当于'except'，后面要用'him'，就像说'except me'一样。",
        encourage: "这个语法点确实很高级，你能尝试就很棒了！慢慢来~"
    },
    {
        q: "The manager wants ___ to complete the report by Friday.",
        options: ["you and I", "you and me", "I and you", "me and you"],
        answer: "you and me",
        explain: "这里用'you and me'，因为是经理想要'你我'完成报告，英语习惯把'you'放前面。",
        encourage: "顺序和形式都很重要呢！你已经注意到这一点了，真不错！"
    },
    {
        q: "___ being late caused problems for everyone.",
        options: ["They", "Them", "Their", "Theirs"],
        answer: "Their",
        explain: "这里用'their'表示'他们的迟到'，就像说'their mistake'一样。",
        encourage: "动名词前的代词形式不容易，但你的思考很有逻辑！继续加油！"
    },
    {
        q: "The responsibility is ___ to bear.",
        options: ["your", "yours", "you", "yourself"],
        answer: "yours",
        explain: "这里用'yours'表示'你的责任'，就像说'this book is yours'一样。",
        encourage: "名词性物主代词用得对！这个有点难的概念你已经掌握啦！"
    },
    {
        q: "___ is certain that the meeting will be postponed.",
        options: ["It", "He", "They", "We"],
        answer: "It",
        explain: "这里用'It'开头，就像说'It is raining'一样，是固定用法。",
        encourage: "形式主语用对啦！这个抽象的用法你已经理解了，真厉害！"
    },
    {
        q: "The committee members voted among ___.",
        options: ["they", "them", "themselves", "their"],
        answer: "themselves",
        explain: "这里用'themselves'表示'他们自己之间'投票。",
        encourage: "反身代词用得恰到好处！这个语法点不容易，但你的理解很到位！"
    },
    {
        q: "___ who arrive early will get the best seats.",
        options: ["Them", "They", "Those", "These"],
        answer: "Those",
        explain: "这里用'Those'指代'那些人'，后面说明是'早到的人'。",
        encourage: "指示代词引导从句完全正确！这个高级语法点你已经掌握啦！"
    },
    {
        q: "The prize will be divided between you and ___.",
        options: ["he", "him", "his", "himself"],
        answer: "him",
        explain: "这里用'him'，因为'between'后面总是用'me, him, her'这样的形式。",
        encourage: "介词后的代词形式完全正确！这个重要规则你已经记住啦！"
    },
    {
        q: "___ knowledge of the subject impressed everyone.",
        options: ["He", "Him", "His", "Himself"],
        answer: "His",
        explain: "这里用'his'表示'他的知识'，就像'his idea'一样表示所属。",
        encourage: "所有格形容词用得准确！这个概念你已经完全掌握啦！"
    },
    {
        q: "The results surprised no one more than ___.",
        options: ["I", "me", "myself", "mine"],
        answer: "me",
        explain: "这里用'me'，因为'than'后面通常用这个形式。",
        encourage: "比较结构中的代词选对啦！这个语法点你已经完全理解了！"
    },
    {
        q: "___ of the students has completed the assignment.",
        options: ["Each", "Every", "All", "Both"],
        answer: "Each",
        explain: "这里用'Each'表示'每一个'学生，后面跟单数动词'has'。",
        encourage: "不定代词与动词一致关系掌握得很好！这个细节你都注意到啦！"
    },
    {
        q: "The teacher asked ___ students to hand in ___ assignments.",
        options: ["we, our", "us, our", "our, us", "us, us"],
        answer: "us, our",
        explain: "第一个用'us'(老师问我们)，第二个用'our'表示'我们的作业'。",
        encourage: "不同形式的连续使用完全正确！这个复杂的结构难不倒你！"
    },
    {
        q: "___ is raining heavily outside.",
        options: ["It", "There", "That", "This"],
        answer: "It",
        explain: "说天气时总是用'It'开头，就像'It is sunny'一样。",
        encourage: "非人称代词用对啦！这个固定用法你已经记住啦！"
    },
    {
        q: "The team celebrated ___ victory.",
        options: ["they", "them", "their", "theirs"],
        answer: "their",
        explain: "这里用'their'表示'他们的胜利'，团队共同拥有的东西。",
        encourage: "团队所有格用得完全正确！集体名词的用法你已经掌握啦！"
    }
];

function showTab(tabId) {
    // Hide all tab contents
    document.querySelectorAll('.tab-content').forEach(tab => {
        tab.classList.remove('active');
    });
    
    // Deactivate all tabs
    document.querySelectorAll('.tab').forEach(tab => {
        tab.classList.remove('active');
    });
    
    // Show selected tab content
    document.getElementById(tabId).classList.add('active');
    
    // Activate selected tab
    event.currentTarget.classList.add('active');
    
    // If history tab is selected, load history
    if (tabId === 'history') {
        loadHistory();
    }
}

function submitQuiz() {
    const name = document.getElementById('name').value;
    const form = document.getElementById('form').value;
    
    if (!name || !form) {
        alert("请填写完整的个人信息！");
        return;
    }
    
    let score = 0;
    let results = [];
    let unanswered = 0;
    
    questions.forEach((q, index) => {
        const selected = document.querySelector(`input[name="q${index}"]:checked`);
        const isCorrect = selected && selected.value === q.answer;
        
        if (isCorrect) score++;
        if (!selected) unanswered++;
        
        results.push({
            question: q.q,
            selected: selected ? selected.value : "未作答",
            correct: q.answer,
            isCorrect: isCorrect,
            explain: q.explain,
            encourage: q.encourage
        });
    });
    
    // Save the attempt to history
    saveAttempt(name, form, score, results);
    
    // Display results
    displayResults(name, form, score, results, unanswered);
}

function displayResults(name, form, score, results, unanswered) {
    let output = `
        <h3>名字: ${name}</h3>
        <h3>年级: ${form}</h3>
        <h3>得分: <span class="${score >= 15 ? 'correct' : 'incorrect'}">${score} / 20</span></h3>
        ${unanswered > 0 ? `<p>注意：你有 ${unanswered} 题没有作答</p>` : ''}
        <p>${getFeedback(score)}</p>
        <hr>
    `;
    
    results.forEach((r, index) => {
        output += `
            <div class="question">
                <p><strong>第${index + 1}题：${r.isCorrect ? '正确 ✅' : '错误 ❌'}</strong></p>
                <p>题目: ${r.question}</p>
                ${!r.isCorrect ? `<p>你的答案: <span class="incorrect">${r.selected}</span></p>` : ''}
                <p>正确答案: <span class="correct">${r.correct}</span></p>
                <p>解释: ${r.explain}</p>
                <p>鼓励: ${r.encourage}</p>
            </div>
        `;
    });
    
    document.getElementById('result').innerHTML = output;
    document.getElementById('result').classList.remove('hidden');
    
    // Scroll to results
    document.getElementById('result').scrollIntoView({ behavior: 'smooth' });
}

function getFeedback(score) {
    if (score === 20) {
        return "太厉害啦！全对耶！你的代词用得跟母语者一样棒！🎉 给自己点个赞吧！";
    } else if (score >= 17) {
        return "成绩很不错哦！只有几个小地方需要注意，你已经掌握大部分内容啦！✨";
    } else if (score >= 14) {
        return "挺好的！基本要点都掌握了，错题看看解释，下次会更好哒！😊";
    } else if (score >= 10) {
        return "有进步空间哦！错题都是学习机会，慢慢来，你会越来越棒的！💪";
    } else {
        return "第一次做这样的题吧？别担心！每个人都是这样进步的，多做几次就会好很多啦！🌱";
    }
}

function saveAttempt(name, form, score, results) {
    const attempts = JSON.parse(localStorage.getItem('pronounQuizAttempts') || '[]');
    const attempt = {
        date: new Date().toLocaleString(),
        name,
        form,
        score,
        results
    };
    
    attempts.unshift(attempt); // Add new attempt at beginning
    localStorage.setItem('pronounQuizAttempts', JSON.stringify(attempts));
}

function loadHistory() {
    const attempts = JSON.parse(localStorage.getItem('pronounQuizAttempts') || '[]');
    const historyList = document.getElementById('historyList');
    
    if (attempts.length === 0) {
        historyList.innerHTML = "<p>你还没有任何测验记录，快去做测验吧！</p>";
        return;
    }
    
    let html = "";
    attempts.forEach((attempt, index) => {
        html += `
            <div class="question" style="margin-bottom: 20px; padding: 15px; background: white; border-radius: 8px;">
                <h3>测验 #${index + 1} - ${attempt.date}</h3>
                <p>姓名: ${attempt.name} | 年级: ${attempt.form}</p>
                <p>得分: <strong>${attempt.score} / 20</strong></p>
                <button onclick="viewAttemptDetails(${index})">查看详情</button>
                <div id="attemptDetails${index}" style="display: none; margin-top: 10px;">
                    ${attempt.results.map((r, qIndex) => `
                        <div style="margin-bottom: 15px; padding: 10px; background: ${r.isCorrect ? '#e6ffe6' : '#ffe6e6'}; border-radius: 5px;">
                            <p><strong>第${qIndex + 1}题：${r.isCorrect ? '正确 ✅' : '错误 ❌'}</strong></p>
                            <p>题目: ${r.question}</p>
                            ${!r.isCorrect ? `<p>你的答案: ${r.selected}</p>` : ''}
                            <p>正确答案: ${r.correct}</p>
                            <p>解释: ${r.explain}</p>
                            <p>鼓励: ${r.encourage}</p>
                        </div>
                    `).join('')}
                </div>
            </div>
        `;
    });
    
    historyList.innerHTML = html;
}

function viewAttemptDetails(index) {
    const detailsDiv = document.getElementById(`attemptDetails${index}`);
    if (detailsDiv.style.display === 'none') {
        detailsDiv.style.display = 'block';
    } else {
        detailsDiv.style.display = 'none';
    }
}

function saveProgress() {
    const name = document.getElementById('name').value;
    const form = document.getElementById('form').value;
    
    if (!name || !form) {
        alert("请先填写个人信息！");
        return;
    }
    
    const progress = {
        name,
        form,
        answers: []
    };
    
    questions.forEach((q, index) => {
        const selected = document.querySelector(`input[name="q${index}"]:checked`);
        progress.answers.push(selected ? selected.value : null);
    });
    
    localStorage.setItem('pronounQuizProgress', JSON.stringify(progress));
    alert("进度已保存！你可以稍后回来继续完成测验。");
}

function loadProgress() {
    const progress = JSON.parse(localStorage.getItem('pronounQuizProgress'));
    
    if (!progress) {
        alert("没有找到保存的进度！");
        return;
    }
    
    document.getElementById('name').value = progress.name;
    document.getElementById('form').value = progress.form;
    
    progress.answers.forEach((answer, index) => {
        if (answer) {
            const radio = document.querySelector(`input[name="q${index}"][value="${answer}"]`);
            if (radio) radio.checked = true;
        }
    });
    
    alert("进度已加载！你可以继续完成测验。");
}

window.onload = function() {
    const qDiv = document.getElementById('questions');
    questions.forEach((q, index) => {
        const div = document.createElement('div');
        div.className = "question";
        div.innerHTML = `<p><strong>第${index + 1}题.</strong> ${q.q}</p>` +
                        q.options.map(opt => `
                            <label><input type="radio" name="q${index}" value="${opt}"> ${opt}</label><br>
                        `).join('');
        qDiv.appendChild(div);
    });
    
    // Check if there's saved progress
    if (localStorage.getItem('pronounQuizProgress')) {
        if (confirm("检测到有保存的进度，是否加载？")) {
            loadProgress();
        }
    }
}
</script>

</body>
</html>
