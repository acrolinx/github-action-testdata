# Acrolinx NextGen Analyzer Demo Repository

This repository demonstrates the **Acrolinx NextGen Analyzer** GitHub Action, showcasing how to integrate content quality analysis into your GitHub workflows.

## 🎯 What This Demo Shows

This repository contains sample content files and a comprehensive GitHub Actions workflow that demonstrates:

- **Automatic Content Analysis**: Analyzes files on push and pull request events
- **Multiple Analysis Types**: Basic, advanced, markdown-only, and text-only analysis
- **Quality Gates**: Automated quality threshold checking
- **Different Configurations**: Various dialects, tones, and style guides
- **Rich Reporting**: Detailed analysis results and summaries

## 📁 Repository Structure

```
├── .github/workflows/
│   └── acrolinx-analysis.yml    # Main demo workflow
├── markdown/                    # Sample Markdown files
│   ├── acrolinx_benefits.md
│   ├── acrolinx_use_cases.md
│   ├── acrolinx_platform_features.md
│   └── acrolinx_company_profile.md
├── text/                        # Sample text files
    ├── acrolinx_leadership.txt
    ├── acrolinx_customers.txt
    ├── acrolinx_technology.txt
    └── acrolinx_company_overview.txt

```

## 🚀 How to Use This Demo

### Prerequisites

1. **Acrolinx Token**: You need an Acrolinx API token
2. **GitHub Secrets**: Add your token as a repository secret

### Setup

1. **Fork or Clone** this repository
2. **Add Secrets** in your repository settings:
   - Go to Settings → Secrets and variables → Actions
   - Add `ACROLINX_TOKEN` with your Acrolinx API token
3. **Enable Actions** if not already enabled

### Triggering Analysis

#### Automatic Triggers
- **Push Events**: Modify any `.md`, `.txt`, `.rst`, or `.adoc` file and push
- **Pull Requests**: Create a PR with changes to supported file types

#### Manual Triggers
1. Go to Actions → Acrolinx Content Analysis
2. Click "Run workflow"
3. Choose analysis type and configuration:
   - **Full Analysis**: Complete analysis with multiple configurations
   - **Markdown-Only**: Analyze only Markdown files
   - **Text-Only**: Analyze only text files
4. Select dialect, tone, and style guide
5. Click "Run workflow"

## 📊 Analysis Types

### 1. Basic Analysis
- **Trigger**: Push/PR events
- **Scope**: Changed files only
- **Features**: Quality scoring, commit status updates

### 2. Advanced Analysis
- **Trigger**: Manual (full analysis)
- **Scope**: All supported files
- **Features**: Multiple configurations comparison

### 3. Markdown-Only Analysis
- **Trigger**: Manual (markdown-only)
- **Scope**: Only `.md` and `.markdown` files
- **Features**: Focused Markdown content analysis

### 4. Text-Only Analysis
- **Trigger**: Manual (text-only)
- **Scope**: Only `.txt` files
- **Features**: Plain text content analysis

## 🔧 Configuration Options

### Dialects
- `american_english` - American English
- `british_english` - British English

### Tones
- `formal` - Formal writing style
- `informal` - Informal writing style
- `academic` - Academic writing style

### Style Guides
- `ap` - Associated Press Style Guide
- `chicago` - Chicago Manual of Style
- `apa` - American Psychological Association

## 📈 Quality Scoring

The action provides comprehensive quality metrics:

- **Quality Score**: Overall content quality (0-100)
- **Clarity Score**: Readability and comprehension
- **Grammar Score**: Grammar and syntax quality
- **Style Guide Score**: Style guide compliance
- **Tone Score**: Tone appropriateness
- **Terminology Score**: Terminology consistency

### Quality Thresholds
- 🟢 **80+**: Excellent quality
- 🟡 **60-79**: Good quality with room for improvement
- 🔴 **0-59**: Needs significant improvement

## 🎯 Demo Scenarios

### Scenario 1: Content Review
1. Edit a Markdown file in the `markdown/` directory
2. Commit and push your changes
3. Watch the automatic analysis run
4. Check the commit status and workflow results

### Scenario 2: Pull Request Quality Gate
1. Create a new branch
2. Make changes to multiple files
3. Create a pull request
4. Review the analysis results in PR comments

### Scenario 3: Full Repository Analysis
1. Go to Actions → Acrolinx Content Analysis
2. Select "Full Analysis"
3. Choose your preferred configuration
4. Run the workflow
5. Review comprehensive results

### Scenario 4: Quality Threshold Testing
1. Make changes that might lower quality scores
2. Push changes to trigger analysis
3. Check if quality gate passes (threshold: 70)
4. Review detailed feedback for improvement

## 📋 Expected Results

### Push Event Results
- Commit status update with quality score
- Workflow run with detailed analysis
- Quality gate pass/fail indication

### Pull Request Results
- PR comments with analysis summary
- Detailed metrics for each file
- Quality recommendations

### Manual Workflow Results
- Comprehensive analysis report
- Multiple configuration comparisons
- Detailed quality metrics

## 🔗 Related Resources

- **[Acrolinx NextGen Analyzer](https://github.com/acrolinx/nextgen-analyzer)**: Main action repository
- **[Documentation](https://github.com/acrolinx/nextgen-analyzer#readme)**: Complete usage guide
- **[Issues](https://github.com/acrolinx/nextgen-analyzer/issues)**: Report bugs or request features
- **[Discussions](https://github.com/acrolinx/nextgen-analyzer/discussions)**: Community discussions

## 🛠️ Customization

You can customize this demo by:

1. **Adding More Files**: Add your own content files to test
2. **Modifying Thresholds**: Change quality gate thresholds
3. **Adding New Configurations**: Test different dialects and tones
4. **Extending Analysis**: Add more analysis types

## 📞 Support

- **Documentation**: [GitHub README](https://github.com/acrolinx/nextgen-analyzer#readme)
- **Issues**: [GitHub Issues](https://github.com/acrolinx/nextgen-analyzer/issues)
- **Discussions**: [GitHub Discussions](https://github.com/acrolinx/nextgen-analyzer/discussions)

---

**Ready to improve your content quality?** 🚀

Start by triggering the workflow and see how Acrolinx NextGen Analyzer can help improve your content quality!

## License

This project is licensed under the Apache-2.0 License - see the [LICENSE](LICENSE) file
for details.