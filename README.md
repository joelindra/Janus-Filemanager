# Janus File Manager

A modern, feature-rich web-based file manager built with PHP and JavaScript. Janus provides an intuitive interface for managing files and directories on a server through a web browser.

## Features

### File Management
- **Browse & Navigate**: Intuitive file browser with breadcrumb navigation
- **File Operations**: Create, edit, rename, delete files and directories
- **File Editor**: Built-in code editor with syntax highlighting (ACE Editor)
- **File Upload**: Support for single and multiple file uploads
- **File Download**: Direct download functionality
- **Permissions Management**: View and modify file/directory permissions (chmod)
- **Bulk Operations**: Select and perform actions on multiple files

### Terminal Integration
- **Web Terminal**: Integrated terminal emulator (xterm.js) for command execution
- **Command History**: Terminal with full command execution support
- **Real-time Output**: Live command output display

### System Information
- **Server Stats**: Display system information including:
  - Operating system details
  - PHP version
  - Web server information
  - Current user and permissions
  - Disk usage statistics
  - Public HTML directory status

### Advanced Tools
- **Port Scanner**: Network port scanning utility
- **GSC File Scanner**: Scan for Google Search Console verification files
- **Process Viewer**: View running system processes
- **Network Information**: Display network interface and connection details
- **PHP Info**: Quick access to PHP configuration

### User Interface
- **Modern Dark Theme**: GitHub-inspired dark theme
- **Responsive Design**: Works on desktop and mobile devices
- **DataTables Integration**: Sortable, searchable file listing
- **Context Menu**: Right-click context menu for quick actions
- **Breadcrumb Navigation**: Easy directory navigation

## Requirements

- PHP 7.0 or higher
- Web server (Apache, Nginx, etc.)
- Modern web browser with JavaScript enabled
- Optional: PHP Zip extension for archive operations

## Installation

1. Upload `janus-filemanager.php` to your web server directory
2. Ensure the file has appropriate permissions (644 recommended)
3. Access the file manager through your web browser
4. The application will automatically initialize in the current directory

## Usage

### Basic Operations

**Navigate Directories**
- Click on folder names to enter directories
- Use breadcrumb navigation to go back
- Click "Home" button to return to root directory

**File Operations**
- **Create File**: Click "Create File" button, enter filename
- **Create Directory**: Click "Create Directory" button, enter directory name
- **Edit File**: Click on file name or use "Edit" from action menu
- **Rename**: Use "Rename" option from action menu
- **Delete**: Use "Delete" option from action menu (with confirmation)
- **Download**: Use "Download" option from action menu

**Terminal Usage**
- Type commands directly in the terminal panel
- Press Enter to execute commands
- Use `cd` command to change directories
- Standard shell commands are supported

### Advanced Features

**Bulk Operations**
1. Select files using checkboxes
2. Choose action from bulk actions bar
3. Confirm operation

**Permissions Management**
1. Click "Permissions" from file action menu
2. Enter octal permission value (e.g., 0755)
3. Click "Save" to apply

**File Scanner**
- Use "GSC SCAN" tool to find specific file types
- Results displayed in modal with action options

**Port Scanner**
- Click "PORT SCAN" tool
- Enter host and port range
- View scan results

## Technical Details

### Architecture
- **Backend**: PHP with session management
- **Frontend**: Vanilla JavaScript with modern ES6+ features
- **UI Framework**: Bootstrap 5.3.2
- **Editor**: ACE Editor with multiple language support
- **Terminal**: xterm.js for terminal emulation
- **Tables**: DataTables for enhanced table functionality

### API Communication
- All operations use JSON-based API
- Base64 encoded payloads for security
- RESTful action-based endpoints

### Security Considerations
- Session-based directory tracking
- Input validation and sanitization
- Error handling and reporting
- Permission checks before operations

### Browser Compatibility
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Opera (latest)

## File Structure

```
janus-filemanager.php    # Main application file (single-file application)
```

## Limitations

- File size limits depend on PHP `upload_max_filesize` and `post_max_size` settings
- Execution of commands depends on server configuration and disabled functions
- Some features require specific PHP extensions (e.g., ZipArchive for zip operations)

## License

This project is provided as-is for authorized use only. Unauthorized access to computer systems is illegal.

## Disclaimer

This software is intended for legitimate system administration and file management purposes only. Users are responsible for ensuring they have proper authorization before using this tool on any system.

## Support

For issues, questions, or contributions, please refer to the project repository.

## Version

Current Version: 1.0-Stealth

---

**Note**: Always ensure you have proper authorization before using this tool on any server. Maintain appropriate security measures and access controls.

