import React, { useState, useEffect } from 'react';
import { Heart, MessageCircle, Repeat, Share, User, Home, Search, Bell, Mail, Bookmark, Settings, Plus, ArrowLeft, Send } from 'lucide-react';

const SocialChatApp = () => {
  const [currentUser, setCurrentUser] = useState({
    id: 1,
    username: 'johndoe',
    name: 'John Doe',
    avatar: '👨‍💻',
    bio: 'Software developer passionate about creating amazing user experiences',
    followers: 1234,
    following: 567,
    posts: 89
  });

  const [users] = useState([
    {
      id: 1,
      username: 'johndoe',
      name: 'John Doe',
      avatar: '👨‍💻',
      bio: 'Software developer passionate about creating amazing user experiences',
      followers: 1234,
      following: 567,
      posts: 89
    },
    {
      id: 2,
      username: 'sarahtech',
      name: 'Sarah Johnson',
      avatar: '👩‍🔬',
      bio: 'Tech enthusiast and AI researcher',
      followers: 890,
      following: 234,
      posts: 56
    },
    {
      id: 3,
      username: 'mikecreative',
      name: 'Mike Wilson',
      avatar: '🎨',
      bio: 'Digital artist and UI/UX designer',
      followers: 2156,
      following: 678,
      posts: 134
    }
  ]);

  const [posts, setPosts] = useState([
    {
      id: 1,
      userId: 2,
      content: "Just shipped a new AI model that can generate beautiful user interfaces! The future of web development is here 🚀",
      timestamp: new Date(Date.now() - 1000 * 60 * 30),
      likes: 42,
      comments: 8,
      reposts: 12,
      liked: false,
      reposted: false,
      image: null
    },
    {
      id: 2,
      userId: 3,
      content: "Working on a new design system for mobile apps. Clean, minimal, and user-friendly. What do you think about glassmorphism in 2025?",
      timestamp: new Date(Date.now() - 1000 * 60 * 60 * 2),
      likes: 28,
      comments: 15,
      reposts: 5,
      liked: true,
      reposted: false,
      image: null
    },
    {
      id: 3,
      userId: 1,
      content: "Beautiful sunset today! Sometimes you need to step away from the code and appreciate the simple things in life ✨",
      timestamp: new Date(Date.now() - 1000 * 60 * 60 * 5),
      likes: 67,
      comments: 23,
      reposts: 8,
      liked: false,
      reposted: true,
      image: null
    }
  ]);

  const [comments, setComments] = useState([
    {
      id: 1,
      postId: 1,
      userId: 3,
      content: "This looks amazing! Can't wait to try it out",
      timestamp: new Date(Date.now() - 1000 * 60 * 15)
    },
    {
      id: 2,
      postId: 1,
      userId: 1,
      content: "Great work Sarah! The demo looks incredible",
      timestamp: new Date(Date.now() - 1000 * 60 * 10)
    },
    {
      id: 3,
      postId: 2,
      userId: 2,
      content: "Glassmorphism is definitely making a comeback!",
      timestamp: new Date(Date.now() - 1000 * 60 * 30)
    }
  ]);

  const [currentPage, setCurrentPage] = useState('home');
  const [selectedUser, setSelectedUser] = useState(null);
  const [selectedPost, setSelectedPost] = useState(null);
  const [newPostContent, setNewPostContent] = useState('');
  const [newCommentContent, setNewCommentContent] = useState('');
  const [showNewPost, setShowNewPost] = useState(false);

  const getUserById = (id) => users.find(user => user.id === id);

  const formatTime = (timestamp) => {
    const now = new Date();
    const diff = now - timestamp;
    const minutes = Math.floor(diff / (1000 * 60));
    const hours = Math.floor(diff / (1000 * 60 * 60));
    const days = Math.floor(diff / (1000 * 60 * 60 * 24));

    if (minutes < 1) return 'now';
    if (minutes < 60) return `${minutes}m`;
    if (hours < 24) return `${hours}h`;
    return `${days}d`;
  };

  const handleLike = (postId) => {
    setPosts(posts.map(post => 
      post.id === postId 
        ? { 
            ...post, 
            liked: !post.liked, 
            likes: post.liked ? post.likes - 1 : post.likes + 1 
          }
        : post
    ));
  };

  const handleRepost = (postId) => {
    setPosts(posts.map(post => 
      post.id === postId 
        ? { 
            ...post, 
            reposted: !post.reposted, 
            reposts: post.reposted ? post.reposts - 1 : post.reposts + 1 
          }
        : post
    ));
  };

  const handleNewPost = () => {
    if (newPostContent.trim()) {
      const newPost = {
        id: posts.length + 1,
        userId: currentUser.id,
        content: newPostContent,
        timestamp: new Date(),
        likes: 0,
        comments: 0,
        reposts: 0,
        liked: false,
        reposted: false,
        image: null
      };
      setPosts([newPost, ...posts]);
      setNewPostContent('');
      setShowNewPost(false);
    }
  };

  const handleNewComment = (postId) => {
    if (newCommentContent.trim()) {
      const newComment = {
        id: comments.length + 1,
        postId: postId,
        userId: currentUser.id,
        content: newCommentContent,
        timestamp: new Date()
      };
      setComments([...comments, newComment]);
      setPosts(posts.map(post => 
        post.id === postId 
          ? { ...post, comments: post.comments + 1 }
          : post
      ));
      setNewCommentContent('');
    }
  };

  const PostCard = ({ post, showComments = false }) => {
    const user = getUserById(post.userId);
    const postComments = comments.filter(comment => comment.postId === post.id);

    return (
      <div className="bg-white border border-gray-200 rounded-lg p-4 mb-4 hover:shadow-md transition-shadow">
        <div className="flex items-start space-x-3">
          <div 
            className="text-2xl cursor-pointer"
            onClick={() => {
              setSelectedUser(user);
              setCurrentPage('profile');
            }}
          >
            {user.avatar}
          </div>
          <div className="flex-1">
            <div className="flex items-center space-x-2">
              <h3 
                className="font-bold text-gray-900 cursor-pointer hover:underline"
                onClick={() => {
                  setSelectedUser(user);
                  setCurrentPage('profile');
                }}
              >
                {user.name}
              </h3>
              <span className="text-gray-500">@{user.username}</span>
              <span className="text-gray-400">·</span>
              <span className="text-gray-500">{formatTime(post.timestamp)}</span>
            </div>
            
            <p className="mt-2 text-gray-900 leading-relaxed">{post.content}</p>
            
            <div className="flex items-center justify-between mt-4 text-gray-500">
              <button 
                className="flex items-center space-x-2 hover:text-blue-500 transition-colors"
                onClick={() => {
                  setSelectedPost(post);
                  setCurrentPage('post');
                }}
              >
                <MessageCircle size={18} />
                <span>{post.comments}</span>
              </button>
              
              <button 
                className={`flex items-center space-x-2 hover:text-green-500 transition-colors ${
                  post.reposted ? 'text-green-500' : ''
                }`}
                onClick={() => handleRepost(post.id)}
              >
                <Repeat size={18} />
                <span>{post.reposts}</span>
              </button>
              
              <button 
                className={`flex items-center space-x-2 hover:text-red-500 transition-colors ${
                  post.liked ? 'text-red-500' : ''
                }`}
                onClick={() => handleLike(post.id)}
              >
                <Heart size={18} fill={post.liked ? 'currentColor' : 'none'} />
                <span>{post.likes}</span>
              </button>
              
              <button className="flex items-center space-x-2 hover:text-blue-500 transition-colors">
                <Share size={18} />
              </button>
            </div>

            {showComments && (
              <div className="mt-4 border-t pt-4">
                <div className="flex items-center space-x-3 mb-4">
                  <div className="text-xl">{currentUser.avatar}</div>
                  <div className="flex-1 flex items-center space-x-2">
                    <input
                      type="text"
                      placeholder="Write a comment..."
                      className="flex-1 border border-gray-300 rounded-full px-4 py-2 focus:outline-none focus:border-blue-500"
                      value={newCommentContent}
                      onChange={(e) => setNewCommentContent(e.target.value)}
                      onKeyPress={(e) => {
                        if (e.key === 'Enter') {
                          handleNewComment(post.id);
                        }
                      }}
                    />
                    <button
                      onClick={() => handleNewComment(post.id)}
                      className="bg-blue-500 text-white p-2 rounded-full hover:bg-blue-600 transition-colors"
                    >
                      <Send size={16} />
                    </button>
                  </div>
                </div>

                <div className="space-y-3">
                  {postComments.map(comment => {
                    const commentUser = getUserById(comment.userId);
                    return (
                      <div key={comment.id} className="flex items-start space-x-3">
                        <div className="text-lg">{commentUser.avatar}</div>
                        <div className="flex-1 bg-gray-50 rounded-lg p-3">
                          <div className="flex items-center space-x-2 mb-1">
                            <span className="font-medium text-gray-900">{commentUser.name}</span>
                            <span className="text-sm text-gray-500">@{commentUser.username}</span>
                            <span className="text-sm text-gray-400">·</span>
                            <span className="text-sm text-gray-500">{formatTime(comment.timestamp)}</span>
                          </div>
                          <p className="text-gray-900">{comment.content}</p>
                        </div>
                      </div>
                    );
                  })}
                </div>
              </div>
            )}
          </div>
        </div>
      </div>
    );
  };

  const NewPostModal = () => (
    <div className="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center z-50">
      <div className="bg-white rounded-lg p-6 w-full max-w-lg mx-4">
        <div className="flex items-center justify-between mb-4">
          <h2 className="text-xl font-bold">Create Post</h2>
          <button 
            onClick={() => setShowNewPost(false)}
            className="text-gray-500 hover:text-gray-700"
          >
            ✕
          </button>
        </div>
        
        <div className="flex items-start space-x-3">
          <div className="text-2xl">{currentUser.avatar}</div>
          <div className="flex-1">
            <textarea
              placeholder="What's happening?"
              className="w-full p-3 border border-gray-300 rounded-lg resize-none focus:outline-none focus:border-blue-500"
              rows={4}
              value={newPostContent}
              onChange={(e) => setNewPostContent(e.target.value)}
            />
            
            <div className="flex justify-between items-center mt-4">
              <span className="text-sm text-gray-500">
                {280 - newPostContent.length} characters remaining
              </span>
              <button
                onClick={handleNewPost}
                disabled={!newPostContent.trim()}
                className="bg-blue-500 text-white px-6 py-2 rounded-full hover:bg-blue-600 disabled:opacity-50 disabled:cursor-not-allowed transition-colors"
              >
                Post
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  );

  const Sidebar = () => (
    <div className="w-64 bg-white h-screen border-r border-gray-200 p-4 fixed left-0 top-0">
      <h1 className="text-2xl font-bold text-blue-500 mb-8">SocialChat</h1>
      
      <nav className="space-y-2">
        <button 
          onClick={() => setCurrentPage('home')}
          className={`flex items-center space-x-3 w-full p-3 rounded-lg transition-colors ${
            currentPage === 'home' ? 'bg-blue-100 text-blue-600' : 'hover:bg-gray-100'
          }`}
        >
          <Home size={20} />
          <span className="font-medium">Home</span>
        </button>
        
        <button className="flex items-center space-x-3 w-full p-3 rounded-lg hover:bg-gray-100 transition-colors">
          <Search size={20} />
          <span className="font-medium">Explore</span>
        </button>
        
        <button className="flex items-center space-x-3 w-full p-3 rounded-lg hover:bg-gray-100 transition-colors">
          <Bell size={20} />
          <span className="font-medium">Notifications</span>
        </button>
        
        <button className="flex items-center space-x-3 w-full p-3 rounded-lg hover:bg-gray-100 transition-colors">
          <Mail size={20} />
          <span className="font-medium">Messages</span>
        </button>
        
        <button className="flex items-center space-x-3 w-full p-3 rounded-lg hover:bg-gray-100 transition-colors">
          <Bookmark size={20} />
          <span className="font-medium">Bookmarks</span>
        </button>
        
        <button 
          onClick={() => {
            setSelectedUser(currentUser);
            setCurrentPage('profile');
          }}
          className={`flex items-center space-x-3 w-full p-3 rounded-lg transition-colors ${
            currentPage === 'profile' && selectedUser?.id === currentUser.id ? 'bg-blue-100 text-blue-600' : 'hover:bg-gray-100'
          }`}
        >
          <User size={20} />
          <span className="font-medium">Profile</span>
        </button>
        
        <button className="flex items-center space-x-3 w-full p-3 rounded-lg hover:bg-gray-100 transition-colors">
          <Settings size={20} />
          <span className="font-medium">Settings</span>
        </button>
      </nav>
      
      <button
        onClick={() => setShowNewPost(true)}
        className="w-full bg-blue-500 text-white font-bold py-3 rounded-full mt-8 hover:bg-blue-600 transition-colors"
      >
        Post
      </button>
      
      <div className="absolute bottom-4 left-4 right-4">
        <div className="flex items-center space-x-3 p-3 rounded-lg hover:bg-gray-100 cursor-pointer transition-colors">
          <div className="text-2xl">{currentUser.avatar}</div>
          <div className="flex-1">
            <p className="font-bold text-gray-900">{currentUser.name}</p>
            <p className="text-gray-500">@{currentUser.username}</p>
          </div>
        </div>
      </div>
    </div>
  );

  const HomePage = () => (
    <div className="ml-64 min-h-screen bg-gray-50">
      <div className="max-w-2xl mx-auto py-6">
        <div className="bg-white border border-gray-200 rounded-lg p-4 mb-6">
          <div className="flex items-start space-x-3">
            <div className="text-2xl">{currentUser.avatar}</div>
            <button
              onClick={() => setShowNewPost(true)}
              className="flex-1 text-left p-3 bg-gray-50 rounded-lg text-gray-500 hover:bg-gray-100 transition-colors"
            >
              What's happening?
            </button>
          </div>
        </div>
        
        <div>
          {posts.map(post => (
            <PostCard key={post.id} post={post} />
          ))}
        </div>
      </div>
    </div>
  );

  const ProfilePage = () => {
    const user = selectedUser;
    const userPosts = posts.filter(post => post.userId === user.id);

    return (
      <div className="ml-64 min-h-screen bg-gray-50">
        <div className="max-w-2xl mx-auto">
          <div className="bg-gradient-to-r from-blue-400 to-purple-500 h-48"></div>
          
          <div className="bg-white -mt-24 relative">
            <div className="p-6">
              <div className="flex justify-between items-start">
                <div className="text-6xl mt-16">{user.avatar}</div>
                <button
                  onClick={() => setCurrentPage('home')}
                  className="bg-white border border-gray-300 px-4 py-2 rounded-full font-bold hover:bg-gray-50 transition-colors"
                >
                  <ArrowLeft size={16} className="inline mr-2" />
                  Back
                </button>
              </div>
              
              <div className="mt-4">
                <h1 className="text-2xl font-bold text-gray-900">{user.name}</h1>
                <p className="text-gray-500">@{user.username}</p>
                <p className="mt-3 text-gray-900">{user.bio}</p>
                
                <div className="flex items-center space-x-6 mt-4 text-sm">
                  <span className="text-gray-500">
                    <strong className="text-gray-900">{user.following}</strong> Following
                  </span>
                  <span className="text-gray-500">
                    <strong className="text-gray-900">{user.followers}</strong> Followers
                  </span>
                  <span className="text-gray-500">
                    <strong className="text-gray-900">{userPosts.length}</strong> Posts
                  </span>
                </div>
              </div>
            </div>
            
            <div className="border-b border-gray-200">
              <nav className="flex space-x-8 px-6">
                <button className="py-4 border-b-2 border-blue-500 text-blue-600 font-medium">
                  Posts
                </button>
                <button className="py-4 text-gray-500 hover:text-gray-700 font-medium">
                  Replies
                </button>
                <button className="py-4 text-gray-500 hover:text-gray-700 font-medium">
                  Media
                </button>
                <button className="py-4 text-gray-500 hover:text-gray-700 font-medium">
                  Likes
                </button>
              </nav>
            </div>
          </div>
          
          <div className="mt-6">
            {userPosts.map(post => (
              <PostCard key={post.id} post={post} />
            ))}
          </div>
        </div>
      </div>
    );
  };

  const PostPage = () => {
    const post = selectedPost;
    
    return (
      <div className="ml-64 min-h-screen bg-gray-50">
        <div className="max-w-2xl mx-auto py-6">
          <div className="flex items-center space-x-4 mb-6">
            <button
              onClick={() => setCurrentPage('home')}
              className="p-2 rounded-full hover:bg-gray-200 transition-colors"
            >
              <ArrowLeft size={20} />
            </button>
            <h1 className="text-xl font-bold">Post</h1>
          </div>
          
          <PostCard post={post} showComments={true} />
        </div>
      </div>
    );
  };

  return (
    <div className="bg-gray-50 min-h-screen">
      <Sidebar />
      
      {currentPage === 'home' && <HomePage />}
      {currentPage === 'profile' && <ProfilePage />}
      {currentPage === 'post' && <PostPage />}
      
      {showNewPost && <NewPostModal />}
    </div>
  );
};

export default SocialChatApp;
