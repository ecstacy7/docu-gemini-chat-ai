
# AI Document Assistant

A modern document processing platform that allows users to upload documents and ask questions about them using AI.

## Features

- **Document Upload**: Support for PDF, TXT, DOC, DOCX, JPG, JPEG, PNG files
- **Drag & Drop Interface**: Modern, intuitive file upload experience
- **AI-Powered Q&A**: Ask questions about your uploaded documents
- **Real-time Chat**: Interactive chat interface with the AI assistant
- **Backend Health Monitoring**: Real-time status indicator for backend connectivity

## Tech Stack

### Frontend
- React 18 with TypeScript
- Tailwind CSS for styling
- shadcn/ui components
- Lucide React icons
- Sonner for toast notifications

### Backend (Your existing Python backend)
- Flask with CORS support
- SQLite database for document storage
- Google Gemini AI for document analysis
- Support for multiple file formats (PDF, DOC, images)

## Getting Started

### Prerequisites
- Node.js & npm (for frontend)
- Python 3.x (for backend)
- Google Gemini API key

### Frontend Setup
1. Clone this repository
2. Install dependencies: `npm install`
3. Start the development server: `npm run dev`
4. The frontend will be available at `http://localhost:8080`

### Backend Setup (Your existing code)
1. Set up your Python environment
2. Install required packages: `pip install flask flask-cors google-generativeai PyPDF2 python-docx pillow python-dotenv`
3. Create a `.env` file with your Gemini API key: `GEMINI_API_KEY=your_api_key_here`
4. Run the backend: `python app.py`
5. The backend will be available at `http://localhost:5000`

## Key Improvements Made

### Fixed File Upload Issues
- **Persistent File Display**: File information now stays visible even if upload fails
- **Better Error Handling**: Comprehensive error states and user feedback
- **Loading States**: Clear visual feedback during upload and processing
- **State Management**: Proper React state management to prevent UI flickering

### Enhanced User Experience
- **Modern UI**: Clean, responsive design with shadcn/ui components
- **Real-time Feedback**: Toast notifications for all user actions
- **Health Check**: Backend connectivity status indicator
- **Drag & Drop**: Intuitive file upload with visual feedback

### Robust Architecture
- **TypeScript**: Type-safe development
- **Component-based**: Modular, maintainable code structure
- **Error Boundaries**: Graceful error handling throughout the app

## API Endpoints

- `POST /upload`: Upload and process documents
- `POST /chat`: Send questions about uploaded documents
- `GET /health`: Backend health check

## File Support

- **Documents**: PDF, TXT, DOC, DOCX
- **Images**: JPG, JPEG, PNG (with OCR placeholder)
- **Size Limit**: Configurable (displays file size in MB)

## Contributing

This platform integrates with your existing Python backend while providing a modern, React-based frontend experience.
