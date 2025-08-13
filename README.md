# FlashCard Master

A modern, intelligent flashcard application built with JavaScript that helps you master vocabulary through spaced repetition learning. Available as both a web app and a desktop application.

## ✨ Features

- **Two-Sided Cards**: Front shows the word, back shows the translation
- **Interactive Flip**: Click any card to flip between front and back
- **Word Categories**: Organize words into custom categories for better learning structure
- **File Upload**: Upload text files with word pairs (word:translation, one per line)
- **Manual Entry**: Add word pairs manually through the text interface
- **Card Editing**: Edit both sides of any flashcard (word, translation, category)
- **Card Management**: Delete cards you no longer need
- **Swipe Gestures**: Swipe right if you know the word, left if you don't
- **Spaced Repetition**: Intelligent algorithm that shows unknown words more frequently
- **Progress Tracking**: Monitor your learning progress with detailed statistics
- **Data Management**: Import/export your progress and word lists
- **Local Storage**: All progress is saved locally in your browser/device
- **Responsive Design**: Works perfectly on both desktop and mobile devices
- **Desktop App**: Native desktop application with system integration

## 🚀 Download Latest Release

Get the latest desktop version of FlashCard Master here:  
[Download FlashCard Master `.dmg`](https://github.com/Wladyslawtt/FlashMaster/releases/latest)

## OR

## 🚀 Getting Started

### Option 1: Web App
1. **Open the App**: Simply open `index.html` in your web browser
2. **Add Words**: Choose between file upload or manual entry
3. **Start Studying**: Begin with the flashcard interface

### Option 2: Desktop App (Recommended)

#### Prerequisites
- Node.js (version 16 or higher)
- npm or yarn package manager

#### Installation Steps
1. **Install Dependencies**:
   ```bash
   npm install
   ```

2. **Run the App**:
   ```bash
   npm start
   ```

3. **Build Desktop App**:
   ```bash
   # For macOS
   npm run build-mac
   
   # For Windows
   npm run build-win
   
   # For Linux
   npm run build-linux
   ```

## 📚 How to Use

### Adding Words

#### Option 1: File Upload
1. Prepare a text file with word pairs in format: `word:translation` (one per line)
2. Click "Choose File" and select your text file
3. Choose or create a category for the words
4. Click "Process File" to add the words

**Example file format:**
```
hello:hola
good:bueno
thank you:gracias
```

#### Option 2: Manual Entry
1. Type or paste word pairs into the text area (one per line, format: `word:translation`)
2. Choose or create a category for the words
3. Click "Add Words" to add them to your study list

### Using the Flashcards

- **Front Side**: Shows the word to learn
- **Back Side**: Shows the translation/definition
- **Flip Card**: Click anywhere on the card to flip between sides
- **Study Flow**: 
  1. See the word on front
  2. Think of the translation
  3. Click to flip and check your answer
  4. Mark as "Know It" or "Don't Know"

### Managing Your Cards

- **Edit Card**: Click "Edit Card" to modify word, translation, or category
- **Delete Card**: Remove cards you no longer need
- **Category Organization**: Group related words together
- **Progress Tracking**: Monitor learning progress per category

### Managing Categories
- **Create Categories**: Add new categories to organize your vocabulary
- **Delete Categories**: Remove categories (words are moved to "General")
- **Category Filter**: Study words from specific categories only
- **Category Stats**: See word counts for each category

### Studying

- **Click to Flip**: Interactive card flipping for better engagement
- **Swipe Right** (or click "Know It"): Mark the word as known
- **Swipe Left** (or click "Don't Know"): Mark the word as unknown
- **Category Display**: See which category each word belongs to
- Words you don't know will appear more frequently until you master them

### Data Management
- **Export Progress**: Save your progress and word lists as JSON files
- **Import Progress**: Restore your progress from previously exported files
- **Menu Integration**: Use File menu in desktop app for quick access

### Spaced Repetition Algorithm

The app uses an intelligent spaced repetition system:
- **Known words**: Review intervals increase exponentially (1 day, 2 days, 4 days, 8 days, etc.)
- **Unknown words**: Review again within 1 day
- **Mastery**: Words reach level 8+ are considered mastered

## 🏗️ File Structure

```
FlashCard JS/
├── index.html              # Main application interface
├── styles.css              # Styling and responsive design
├── script.js               # Core application logic
├── main.js                 # Electron main process
├── preload.js              # Electron preload script
├── package.json            # Node.js dependencies and build config
├── sample-words.txt        # Example word pairs (word:translation)
└── README.md               # This file
```

## 🖥️ Desktop App Features

### System Integration
- Native macOS/Windows/Linux applications
- System menu bar integration
- Keyboard shortcuts (Cmd/Ctrl+O for import, Cmd/Ctrl+S for export)
- File drag & drop support
- App icon and proper window management

### Enhanced File Operations
- Native file dialogs
- Better file type handling
- Progress backup and restore
- Cross-platform compatibility

## 🌐 Browser Compatibility

- Chrome (recommended)
- Firefox
- Safari
- Edge
- Mobile browsers (iOS Safari, Chrome Mobile)

## 💾 Data Storage

### Web App
- Progress saved in browser's local storage
- Data persists between browser sessions
- No account or internet connection required
- Data stays private on your device

### Desktop App
- Data stored locally on your device
- Automatic backup capabilities
- Import/export functionality
- Cross-device data transfer

## 💡 Tips for Best Results

1. **Use Word Pairs**: Format your input as `word:translation` for best results
2. **Organize by Categories**: Group related words together for better learning
3. **Interactive Learning**: Use the flip functionality to test yourself
4. **Consistency**: Study regularly for optimal retention
5. **Honesty**: Be honest about whether you know a word
6. **Review**: Let the spaced repetition algorithm work - don't rush through words
7. **Backup**: Regularly export your progress to avoid data loss
8. **Edit Cards**: Customize translations and categories as you learn

## 🔧 Technical Details

- **Frontend**: Vanilla JavaScript with modern ES6+ features
- **Desktop**: Electron framework for cross-platform desktop apps
- **Layout**: CSS Grid and Flexbox for responsive design
- **Card Animation**: CSS 3D transforms for smooth card flipping
- **Gestures**: Touch and mouse event handling for swipe gestures
- **Storage**: Local storage API for data persistence
- **Algorithm**: Spaced repetition based on exponential backoff
- **Security**: Context isolation and secure IPC communication

## 🚨 Getting Help

If you encounter any issues:

### Web App
1. Check that your browser supports local storage
2. Ensure JavaScript is enabled
3. Try refreshing the page if the app seems unresponsive
4. Check the browser console for any error messages

### Desktop App
1. Ensure Node.js is properly installed
2. Check that all dependencies are installed (`npm install`)
3. Try running in development mode first (`npm start`)
4. Check the terminal for any error messages
5. Verify file permissions for import/export operations

## 📦 Building from Source

1. **Clone the repository**
2. **Install dependencies**: `npm install`
3. **Run in development**: `npm start`
4. **Build for distribution**: `npm run build`

## 📄 License

This project is open source and available under the MIT License.

---

**Happy Learning! 🎓✨**

*FlashCard Master - Your intelligent vocabulary companion with interactive two-sided cards* 
