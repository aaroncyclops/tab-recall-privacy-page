<!doctype html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
    <title>TabRecall Privacy & Support</title>
    <style>
        :root {
            color-scheme: light dark;
            --background: #f2f2f7;
            --group-bg: #ffffff;
            --label: #111111;
            --secondary-label: #4d4d52;
            --separator: rgba(60, 60, 67, 0.29);
            --accent: #007aff;
            --status: #6e6e73;
            --danger: #ff3b30;
            --max-width: 620px;
        }

        * {
            box-sizing: border-box;
        }

        body {
            margin: 0;
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
            line-height: 1.4;
            min-height: 100dvh;
            background: var(--background);
            color: var(--label);
            padding:
                max(16px, env(safe-area-inset-top))
                max(16px, env(safe-area-inset-right))
                max(18px, env(safe-area-inset-bottom))
                max(16px, env(safe-area-inset-left));
        }

        .page {
            width: min(100%, var(--max-width));
            margin: 0 auto;
        }

        .hero {
            margin: 4px 0 18px;
        }

        h1 {
            margin: 0;
            font-size: 2rem;
            letter-spacing: -0.02em;
            line-height: 1.12;
        }

        .subtitle {
            margin: 10px 0 0;
            color: var(--secondary-label);
            font-size: 1.06rem;
        }

        .group {
            background: var(--group-bg);
            border-radius: 14px;
            overflow: hidden;
            box-shadow: 0 0 0 0.5px var(--separator);
            padding: 12px 14px 14px;
        }

        .group + .group {
            margin-top: 12px;
        }

        h2 {
            margin: 0;
            color: var(--secondary-label);
            font-size: 0.8rem;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 0.02em;
        }

        p {
            margin: 10px 0 0;
        }

        ul {
            margin: 10px 0 0;
            padding-left: 20px;
        }

        li + li {
            margin-top: 6px;
        }

        .field {
            margin-top: 12px;
        }

        label {
            display: block;
            margin-bottom: 6px;
            font-size: 0.95rem;
            font-weight: 600;
        }

        input,
        textarea {
            width: 100%;
            border: 1px solid var(--separator);
            border-radius: 10px;
            background: #ffffff;
            color: inherit;
            padding: 10px 12px;
            font: inherit;
        }

        input {
            min-height: 44px;
        }

        textarea {
            min-height: 128px;
            resize: vertical;
        }

        input:focus-visible,
        textarea:focus-visible,
        button:focus-visible,
        a:focus-visible {
            outline: 2px solid var(--accent);
            outline-offset: 2px;
        }

        .helper {
            margin-top: 10px;
            color: var(--secondary-label);
            font-size: 0.88rem;
        }

        .primaryButton {
            width: 100%;
            min-height: 50px;
            margin-top: 14px;
            border: 0;
            border-radius: 12px;
            background: var(--accent);
            color: #ffffff;
            font: inherit;
            font-weight: 600;
            cursor: pointer;
            -webkit-appearance: none;
            appearance: none;
        }

        .status {
            min-height: 1.2em;
            margin-top: 10px;
            color: var(--status);
            font-size: 0.9rem;
        }

        .status.error {
            color: var(--danger);
        }

        .supportLink {
            margin-top: 10px;
            font-size: 0.92rem;
        }

        a {
            color: var(--accent);
        }

        .meta {
            margin-top: 10px;
            color: var(--status);
            font-size: 0.86rem;
        }

        footer {
            margin-top: 16px;
            text-align: center;
            color: var(--status);
            font-size: 0.84rem;
        }

        @media (min-width: 768px) {
            body {
                padding:
                    max(24px, env(safe-area-inset-top))
                    max(24px, env(safe-area-inset-right))
                    max(24px, env(safe-area-inset-bottom))
                    max(24px, env(safe-area-inset-left));
            }
        }

        @media (prefers-color-scheme: dark) {
            :root {
                --background: #000000;
                --group-bg: #1c1c1e;
                --label: #f2f2f7;
                --secondary-label: #a1a1aa;
                --separator: rgba(84, 84, 88, 0.65);
                --status: #9b9ba1;
            }

            input,
            textarea {
                background: #2c2c2e;
            }
        }
    </style>
</head>
<body>
    <main class="page">
        <header class="hero">
            <h1>TabRecall</h1>
            <p class="subtitle">A simple, privacy-first Safari extension for reopening recently closed tabs.</p>
        </header>

        <section class="group" aria-labelledby="glance-title">
            <h2 id="glance-title">Privacy at a Glance</h2>
            <p>TabRecall stores recently closed tab URLs on your device so you can reopen them quickly. It does not use third-party advertising SDKs and does not send analytics or tracking data from this page.</p>
            <p class="meta">Last updated: February 8, 2026</p>
        </section>

        <section class="group" aria-labelledby="data-title">
            <h2 id="data-title">What Data TabRecall Uses</h2>
            <ul>
                <li>Recently closed tab URLs, used only to power reopen features.</li>
                <li>User preferences such as reopen count, background reopen behavior, and domain exclusions.</li>
            </ul>
            <p>TabRecall does not use this data for profiling, ads, or third-party tracking.</p>
        </section>

        <section class="group" aria-labelledby="storage-title">
            <h2 id="storage-title">How Data Is Stored</h2>
            <p>Data is stored locally in your browser extension storage on your device. This allows TabRecall to function without requiring a cloud account or external backend.</p>
        </section>

        <section class="group" aria-labelledby="controls-title">
            <h2 id="controls-title">Data Retention &amp; Controls</h2>
            <p>You can manage stored data and behavior directly in TabRecall settings:</p>
            <ul>
                <li>Clear recently closed history</li>
                <li>Configure domain exclusions</li>
                <li>Set max recently closed shown</li>
                <li>Reset settings to defaults</li>
            </ul>
        </section>

        <section class="group" aria-labelledby="support-title">
            <h2 id="support-title">Support</h2>
            <p>If you need help, send a support email using the form below.</p>
            <form id="supportForm" novalidate>
                <div class="field">
                    <label for="name">Name (optional)</label>
                    <input id="name" name="name" type="text" autocomplete="name">
                </div>

                <div class="field">
                    <label for="email">Email (optional, recommended)</label>
                    <input id="email" name="email" type="email" autocomplete="email">
                </div>

                <div class="field">
                    <label for="subject">Subject (required)</label>
                    <input id="subject" name="subject" type="text" required>
                </div>

                <div class="field">
                    <label for="message">Message (required)</label>
                    <textarea id="message" name="message" required></textarea>
                </div>

                <p class="helper">Submitting opens your mail app; nothing is sent from this page directly.</p>
                <button class="primaryButton" type="submit">Open Mail App</button>
                <p id="formStatus" class="status" aria-live="polite"></p>
            </form>

            <p class="supportLink">Prefer direct email? <a href="mailto:aaronfimple@gmail.com">aaronfimple@gmail.com</a></p>
        </section>

        <footer>
            <p>Aaron Fimple 2026 - v1.0</p>
            <p><a href="mailto:aaronfimple@gmail.com">aaronfimple@gmail.com</a></p>
        </footer>
    </main>

    <script>
        (function () {
            const supportForm = document.getElementById("supportForm");
            const nameInput = document.getElementById("name");
            const emailInput = document.getElementById("email");
            const subjectInput = document.getElementById("subject");
            const messageInput = document.getElementById("message");
            const statusElement = document.getElementById("formStatus");
            const supportEmail = "aaronfimple@gmail.com";

            function setStatus(text, isError) {
                statusElement.textContent = text;
                statusElement.classList.toggle("error", Boolean(isError));
            }

            supportForm.addEventListener("submit", function (event) {
                event.preventDefault();
                setStatus("", false);

                const name = nameInput.value.trim();
                const email = emailInput.value.trim();
                const subject = subjectInput.value.trim();
                const message = messageInput.value.trim();

                if (!subject) {
                    setStatus("Please enter a subject.", true);
                    subjectInput.focus();
                    return;
                }

                if (!message) {
                    setStatus("Please enter a message.", true);
                    messageInput.focus();
                    return;
                }

                if (email && !emailInput.checkValidity()) {
                    setStatus("Please enter a valid email address.", true);
                    emailInput.focus();
                    return;
                }

                const bodyLines = [
                    "TabRecall Support Request",
                    "",
                    "Name: " + (name || "Not provided"),
                    "Email: " + (email || "Not provided"),
                    "",
                    "Message:",
                    message
                ];

                const mailtoURL = "mailto:" + supportEmail +
                    "?subject=" + encodeURIComponent("[TabRecall] " + subject) +
                    "&body=" + encodeURIComponent(bodyLines.join("\n"));

                setStatus("Opening your mail app...", false);
                window.location.href = mailtoURL;
            });
        }());
    </script>
</body>
</html>
