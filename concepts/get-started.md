# <a name="getting-started-building-microsoft-graph-apps"></a><span data-ttu-id="59639-101">开始生成 Microsoft Graph 应用</span><span class="sxs-lookup"><span data-stu-id="59639-101">Getting started building Microsoft Graph apps</span></span>

<span data-ttu-id="59639-p101">此部分中的文章提供了有关如何跨越各种语言和开发平台生成连接到 Microsoft Graph 的应用的详细指南。每篇文章从相应平台的初学者项目示例开始，引导你添加对用户进行身份验证并创建示例请求以使 Microsoft Graph 从其帐户发送电子邮件的功能。完成后的项目与该平台的 [Microsoft Graph 存储库中的 Connect 示例](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect) 一样。</span><span class="sxs-lookup"><span data-stu-id="59639-p101">The articles in this section provide detailed guidance on how to build apps that connect to Microsoft Graph across a variety of languages and development platforms. Each article starts with a sample starter project for the appropriate platform, and walks you through adding functionality that authenticates the user and makes a sample request to have Microsoft Graph send an email from their account. The completed project is identical to the [Connect sample in the Microsoft Graph repo](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect) for that platform.</span></span>

<span data-ttu-id="59639-105">选择涉及所选身份验证程序和开发平台的文章，然后开始连接到 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="59639-105">Choose the article that covers the authentication provider and development platform of your choice, and get started connecting to Microsoft Graph.</span></span>

<span data-ttu-id="59639-106">可以按照涉及所选开发平台的文章中的步骤操作，或者，若要快速创建并运行有效的解决方案，请尝试使用 [快速入门](https://developer.microsoft.com/graph/quick-start) 体验。</span><span class="sxs-lookup"><span data-stu-id="59639-106">You can follow the steps in the article that covers the development platform that you choose, or, to quickly get a working solution up and running, try out the [quick start](https://developer.microsoft.com/graph/quick-start) experience.</span></span>

<span data-ttu-id="59639-p102">若要浏览已完成的 Connect 示例，请访问 GitHub 上的 [Microsoft Graph](https://github.com/microsoftgraph)。下表按验证提供程序和平台列出了示例，并标注了是使用 REST 还是使用 Microsoft Graph 客户端库连接到 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="59639-p102">To explore the finished Connect samples, see [Microsoft Graph](https://github.com/microsoftgraph) in GitHub. The following table lists the samples by authentication provider and platform, and notes whether they connect to Microsoft Graph using REST or a Microsoft Graph client library.</span></span>

<table>
  <tr>
    <th><span data-ttu-id="59639-109">平台</span><span class="sxs-lookup"><span data-stu-id="59639-109">Platform</span></span></th>
    <th><span data-ttu-id="59639-110">Azure AD 终结点</span><span class="sxs-lookup"><span data-stu-id="59639-110">Azure AD endpoint</span></span></th> 
    <th><span data-ttu-id="59639-111">Azure AD v2.0 终结点</span><span class="sxs-lookup"><span data-stu-id="59639-111">Azure AD v2.0 endpoint</span></span></th>
  </tr>
  <tr>
    <td><span data-ttu-id="59639-112">Android</span><span class="sxs-lookup"><span data-stu-id="59639-112">Android</span></span></td>
    <td><span data-ttu-id="59639-113">
        <a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">SDK 示例</a>
    </span><span class="sxs-lookup"><span data-stu-id="59639-113">
        <a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">SDK sample</a>
    </span></span></td> 
        <td><span data-ttu-id="59639-114">
                <a href="https://github.com/microsoftgraph/android-java-connect-sample">SDK 示例</a>或 ¶<a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">REST 示例</a>
    </span><span class="sxs-lookup"><span data-stu-id="59639-114">
                <a href="https://github.com/microsoftgraph/android-java-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="59639-115">AngularJS</span><span class="sxs-lookup"><span data-stu-id="59639-115">AngularJS</span></span></td>
    <td><span data-ttu-id="59639-116">
        <a href="https://github.com/microsoftgraph/angular-connect-rest-sample/tree/last_v1_auth">REST 示例</a>
    </span><span class="sxs-lookup"><span data-stu-id="59639-116">
        <a href="https://github.com/microsoftgraph/angular-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td> 
        <td><span data-ttu-id="59639-117">
        <a href="https://github.com/microsoftgraph/angular-connect-sample">SDK 示例</a>或 ¶<a href="https://github.com/microsoftgraph/angular-connect-rest-sample">REST 示例</a>
    </span><span class="sxs-lookup"><span data-stu-id="59639-117">
        <a href="https://github.com/microsoftgraph/angular-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/angular-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="59639-118">ASP.NET</span><span class="sxs-lookup"><span data-stu-id="59639-118">ASP.NET</span></span></td>
    <td><span data-ttu-id="59639-119">
        <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth">REST 示例</a>
    </span><span class="sxs-lookup"><span data-stu-id="59639-119">
        <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="59639-120">
        <a href="https://github.com/microsoftgraph/aspnet-connect-sample">SDK 示例</a>或 ¶<a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">REST 示例</a>
    </span><span class="sxs-lookup"><span data-stu-id="59639-120">
        <a href="https://github.com/microsoftgraph/aspnet-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="59639-121">iOS (Obj-C)</span><span class="sxs-lookup"><span data-stu-id="59639-121">iOS (Obj-C)</span></span></td>
    <td><span data-ttu-id="59639-122">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">REST 示例</a>
    </span><span class="sxs-lookup"><span data-stu-id="59639-122">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="59639-123">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">SDK 示例</a>
    </span><span class="sxs-lookup"><span data-stu-id="59639-123">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="59639-124">iOS (Swift)</span><span class="sxs-lookup"><span data-stu-id="59639-124">iOS (Swift)</span></span></td>
    <td><span data-ttu-id="59639-125">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">REST 示例</a>
    </span><span class="sxs-lookup"><span data-stu-id="59639-125">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="59639-126">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-sample">SDK 示例</a>
    </span><span class="sxs-lookup"><span data-stu-id="59639-126">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="59639-127">NodeJS</span><span class="sxs-lookup"><span data-stu-id="59639-127">NodeJS</span></span></td>
    <td><span data-ttu-id="59639-128">
        <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">REST 示例</a>
    </span><span class="sxs-lookup"><span data-stu-id="59639-128">
        <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td>    
        <span data-ttu-id="59639-129"><a href="https://github.com/microsoftgraph/nodejs-connect-sample">SDK 示例</a>或 <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">REST 示例</a>
    </span><span class="sxs-lookup"><span data-stu-id="59639-129"><a href="https://github.com/microsoftgraph/nodejs-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="59639-130">PHP</span><span class="sxs-lookup"><span data-stu-id="59639-130">PHP</span></span></td>
    <td><span data-ttu-id="59639-131">
        <a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">REST 示例</a>
    </span><span class="sxs-lookup"><span data-stu-id="59639-131">
        <a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="59639-132">
            <a href="https://github.com/microsoftgraph/php-connect-sample">SDK 示例</a>或 ¶<a href="https://github.com/microsoftgraph/php-connect-rest-sample">REST 示例</a>
    </span><span class="sxs-lookup"><span data-stu-id="59639-132">
            <a href="https://github.com/microsoftgraph/php-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/php-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="59639-133">Python</span><span class="sxs-lookup"><span data-stu-id="59639-133">Python</span></span></td>
    <td><span data-ttu-id="59639-134">
        <a href="https://github.com/microsoftgraph/python3-connect-rest-sample">REST 示例</a>
    </span><span class="sxs-lookup"><span data-stu-id="59639-134">
        <a href="https://github.com/microsoftgraph/python3-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td>
    </td> 
  </tr>
  <tr>
    <td><span data-ttu-id="59639-135">Ruby</span><span class="sxs-lookup"><span data-stu-id="59639-135">Ruby</span></span></td>
    <td><span data-ttu-id="59639-136">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">REST 示例</a>
    </span><span class="sxs-lookup"><span data-stu-id="59639-136">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="59639-137">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">REST 示例</a>
    </span><span class="sxs-lookup"><span data-stu-id="59639-137">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="59639-138">UWP</span><span class="sxs-lookup"><span data-stu-id="59639-138">UWP</span></span></td>
    <td><span data-ttu-id="59639-139">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">REST 示例</a>
    </span><span class="sxs-lookup"><span data-stu-id="59639-139">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="59639-140">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">SDK 示例</a>或 ¶<a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">REST 示例</a>
    </span><span class="sxs-lookup"><span data-stu-id="59639-140">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="59639-141">Xamarin</span><span class="sxs-lookup"><span data-stu-id="59639-141">Xamarin</span></span></td>
    <td>
    </td>     
    <td><span data-ttu-id="59639-142">
        <a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">SDK 示例</a>
    </span><span class="sxs-lookup"><span data-stu-id="59639-142">
        <a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
</table>

## <a name="see-also"></a><span data-ttu-id="59639-143">另请参阅</span><span class="sxs-lookup"><span data-stu-id="59639-143">See also</span></span>
- <span data-ttu-id="59639-144">请在我们的 [API Explorer](https://developer.microsoft.com/graph/graph-explorer) 中尝试使用示例 REST 调用。</span><span class="sxs-lookup"><span data-stu-id="59639-144">Try out sample REST calls in our [API Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- [<span data-ttu-id="59639-145">Azure AD 终结点文档</span><span class="sxs-lookup"><span data-stu-id="59639-145">Azure AD endpoint documentation</span></span>](https://azure.microsoft.com/documentation/services/active-directory/)
- [<span data-ttu-id="59639-146">Azure AD v2.0 终结点文档</span><span class="sxs-lookup"><span data-stu-id="59639-146">Azure AD v2.0 endpoint documentation</span></span>](https://azure.microsoft.com/documentation/articles/?service=active-directory&term=azure+ad+v2.0)
