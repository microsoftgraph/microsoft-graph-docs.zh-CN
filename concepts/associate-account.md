---
title: 将 Office 365 帐户与 Azure AD 相关联以创建和管理应用
description: '若要使用 Microsoft Azure Active Directory (Azure AD) 验证应用，必须在 Azure AD 中注册应用。这也是存储 Office 365 用户帐户和应用信息的位置。必须有 Microsoft Azure 订阅，才能通过 Azure 门户管理 Azure AD。可以使用 Microsoft Azure 门户管理用户、角色和应用。 '
localization_priority: Normal
ms.openlocfilehash: 815cc80fa8d25f52ac05a1bf80f9e9dfa89b9b4d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880155"
---
# <a name="associate-your-office-365-account-with-azure-ad-to-create-and-manage-apps"></a><span data-ttu-id="49fa0-106">将 Office 365 帐户与 Azure AD 关联以创建和管理应用</span><span class="sxs-lookup"><span data-stu-id="49fa0-106">Associate your Office 365 account with Azure AD to create and manage apps</span></span>

<span data-ttu-id="49fa0-p102">若要使用 Microsoft Azure Active Directory (Azure AD) 验证应用，必须在 Azure AD 中注册应用。这也是存储 Office 365 用户帐户和应用信息的位置。必须有 Microsoft Azure 订阅，才能通过 Azure 门户管理 Azure AD。可以使用 Microsoft Azure 门户管理用户、角色和应用。</span><span class="sxs-lookup"><span data-stu-id="49fa0-p102">To authenticate your applications using Microsoft Azure Active Directory (Azure AD), you need to register them in Azure AD. This is where Office 365 user account and application information is stored. To manage Azure AD through the Azure portal, you need a Microsoft Azure subscription. You can use the portal in Microsoft Azure to manage users, roles, and apps.</span></span> 

<span data-ttu-id="49fa0-111">本文介绍了如何将 Office 365 帐户和 Azure AD 关联以创建和管理应用。</span><span class="sxs-lookup"><span data-stu-id="49fa0-111">This article shows you how to associate your Office 365 account with Azure AD to create and manage apps.</span></span>

 ><span data-ttu-id="49fa0-p103">**注意：** 本文将 Azure AD 用作应用的身份验证提供程序。如果使用的是 Azure AD v2.0 终结点，则无需执行此步骤。有关详细信息，请参阅 [Microsoft Graph 的应用身份验证](auth-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="49fa0-p103">**Note:** This article uses Azure AD as the authentication provider for your app. If you're using the Azure AD v2.0 endpoint, you don't need to perform this step. For more information, see [App authentication with Microsoft Graph](auth-overview.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49fa0-115">先决条件</span><span class="sxs-lookup"><span data-stu-id="49fa0-115">Prerequisites</span></span>

<span data-ttu-id="49fa0-116">**Office 365 商业版帐户**</span><span class="sxs-lookup"><span data-stu-id="49fa0-116">**Office 365 for business account**</span></span>

<span data-ttu-id="49fa0-117">如果没有现成的 Office 365 商业版帐户，则可以：</span><span class="sxs-lookup"><span data-stu-id="49fa0-117">If you don't have an existing Office 365 for business account, you can:</span></span>

- <span data-ttu-id="49fa0-118">注册上面列出的 [Office 365 商业版计划](https://products.office.com/zh-CN/business/compare-office-365-for-business-plans)，或</span><span class="sxs-lookup"><span data-stu-id="49fa0-118">Sign up for an [Office 365 for business plans](https://products.office.com/zh-CN/business/compare-office-365-for-business-plans) listed above, or</span></span>
- <span data-ttu-id="49fa0-119">[参加 Office 365 开发人员计划并获取为期 1 年的免费 Office 365 订阅](https://aka.ms/devprogramsignup)。</span><span class="sxs-lookup"><span data-stu-id="49fa0-119">[Join the Office 365 Developer Program and get a free 1 year subscription to Office 365](https://aka.ms/devprogramsignup).</span></span>

<span data-ttu-id="49fa0-120">**Microsoft Azure 订阅**</span><span class="sxs-lookup"><span data-stu-id="49fa0-120">**Microsoft Azure subscription**</span></span> 

- <span data-ttu-id="49fa0-121">如果有现成的 Microsoft Azure 订阅，则可以将它与 Office 365 商业版订阅相关联。</span><span class="sxs-lookup"><span data-stu-id="49fa0-121">If you can have an existing Microsoft Azure subscription, you can associate your Office 365 for business subscription with it.</span></span> 

- <span data-ttu-id="49fa0-122">否则，您将需要新建一个 Azure 订阅，并将它与您的 Office 365 帐户相关联以便注册和管理应用。</span><span class="sxs-lookup"><span data-stu-id="49fa0-122">Otherwise, you'll need to create a new Azure subscription and associate it with your Office 365 account in order to register and manage apps.</span></span>


<!---<a name="bk_AssociateExistingAzureSubscription"> </a>-->

## <a name="to-associate-an-existing-azure-subscription-with-your-office-365-account"></a><span data-ttu-id="49fa0-123">关联现有 Azure 订阅和 Office 365 帐户的具体步骤</span><span class="sxs-lookup"><span data-stu-id="49fa0-123">To associate an existing Azure subscription with your Office 365 account</span></span>


1. <span data-ttu-id="49fa0-124">使用现有 Azure 凭据（例如，user@live.com 等 Microsoft ID）登录 [Microsoft Azure 门户](https://portal.azure.com)。</span><span class="sxs-lookup"><span data-stu-id="49fa0-124">Log on to the  [Microsoft Azure portal](https://portal.azure.com) with your existing Azure credentials (for example, your Microsoft ID such as user@live.com).</span></span>
        
2. <span data-ttu-id="49fa0-125">依次选择“Active Directory”\*\*\*\* 节点、“目录”\*\*\*\* 选项卡和屏幕底部的“新建”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="49fa0-125">Select the  **Active Directory** node, then select the **Directory** tab and, at the bottom of the screen, select **New**.</span></span> 
     
4. <span data-ttu-id="49fa0-126">在“**新建**”菜单中，依次选择“**Active Directory**” > “**目录**” > “**自定义创建**”。</span><span class="sxs-lookup"><span data-stu-id="49fa0-126">On the **New** menu, select **Active Directory** > **Directory** > **Custom Create**.</span></span>
    
5. <span data-ttu-id="49fa0-p104">在“**添加目录**”中，在“**目录**”下拉框中，选择“**使用现有目录**”。单击“**我已准备好注销**”，然后选中右下角的复选标记。</span><span class="sxs-lookup"><span data-stu-id="49fa0-p104">In **Add directory**, in the **Directory** dropdown box, select  **Use existing directory**. Check **I am ready to be signed out**, and then select the check mark in the lower-right corner.</span></span> 
    
    <span data-ttu-id="49fa0-129">这样，可以返回到 Azure 门户。</span><span class="sxs-lookup"><span data-stu-id="49fa0-129">This brings you back to the Azure portal.</span></span>
        
3. <span data-ttu-id="49fa0-130">使用 Office 365 帐户信息登录。</span><span class="sxs-lookup"><span data-stu-id="49fa0-130">Log in with your Office 365 account information.</span></span> 
    
    <span data-ttu-id="49fa0-131">系统将提示是否要通过 Azure 使用目录。</span><span class="sxs-lookup"><span data-stu-id="49fa0-131">You will be prompted whether to use your directory with Azure.</span></span> 
    
    ><span data-ttu-id="49fa0-132">**重要说明：** 若要将 Office 365 帐户与 Azure AD 相关联，则需要具有全局管理员权限的 Office 365 商业版帐户。</span><span class="sxs-lookup"><span data-stu-id="49fa0-132">**Important:** To associate your Office 365 account with Azure AD, you'll need  an Office 365 business account with global administrator privileges.</span></span> 
    
        
4. <span data-ttu-id="49fa0-133">依次选择“**继续**”和“**立即注销**”。</span><span class="sxs-lookup"><span data-stu-id="49fa0-133">Select  **continue**, and then **Sign out now**.</span></span>
        
5. <span data-ttu-id="49fa0-p105">关闭浏览器，然后重新打开[门户](https://manage.windowsazure.com)。否则，你将收到访问被拒绝错误。</span><span class="sxs-lookup"><span data-stu-id="49fa0-p105">Close the browser and reopen the  [portal](https://manage.windowsazure.com). Otherwise, you will get an access denied error.</span></span>
    
        
6. <span data-ttu-id="49fa0-p106">使用现有的 Azure 凭据（例如，诸如 user@live.com 之类的 Microsoft ID）重新登录。转到“**Active Directory**”节点，在“**目录**”下，应该会看到 Office 365 帐户被列出。</span><span class="sxs-lookup"><span data-stu-id="49fa0-p106">Log on again with your existing Azure credentials (for example, your Microsoft ID such as user@live.com). Go to the  **Active Directory** node and, under **Directory**, you should now see your Office 365 account listed.</span></span>
    

<!--<a name="bk_AssociateNewAzureSubscription"> </a>-->

## <a name="to-create-a-new-azure-subscription-and-associate-it-with-your-office-365-account"></a><span data-ttu-id="49fa0-138">若要新建 Azure 订阅并将它与 Office 365 帐户相关联</span><span class="sxs-lookup"><span data-stu-id="49fa0-138">To create a new Azure subscription and associate it with your Office 365 account</span></span>


1. <span data-ttu-id="49fa0-p107">登录 Office 365。在“**主页**”中，选择“**管理员**”图标，打开 Office 365 管理中心。</span><span class="sxs-lookup"><span data-stu-id="49fa0-p107">Log on to Office 365. From the **Home** page, select the **Admin** icon to open the Office 365 admin center.</span></span>
2. <span data-ttu-id="49fa0-141">在菜单页中，沿着页面左侧，向下滚动至“**管理员**”，然后选择“**Azure AD**”。</span><span class="sxs-lookup"><span data-stu-id="49fa0-141">In the menu page along the left side of the page, scroll down to **Admin** and select **Azure AD**.</span></span>

    ><span data-ttu-id="49fa0-142">**重要说明：** 若要打开 Office 365 管理中心，则需要具有全局管理员权限的 Office 365 商业版帐户。</span><span class="sxs-lookup"><span data-stu-id="49fa0-142">**Important:** To open the Office 365 admin center, and access Azure AD, you'll need  an Office 365 business account with global administrator privileges.</span></span> 
    
3. <span data-ttu-id="49fa0-143">新建一个订阅。</span><span class="sxs-lookup"><span data-stu-id="49fa0-143">Create a new subscription.</span></span>
        
    <span data-ttu-id="49fa0-p108">如果使用 Office 365 的试用版，您将看到一条消息告诉您 Azure AD 仅限使用付费服务的客户使用。仍然可以免费创建 30 天试用 Azure 订阅，但需要执行几个额外的步骤：</span><span class="sxs-lookup"><span data-stu-id="49fa0-p108">If you're using a trial version of Office 365, you'll see a message telling you that Azure AD is limited to customers with paid services. You can still create a trial 30-day Azure subscription at no charge, but you'll need to perform a few extra steps:</span></span>
    
    1. <span data-ttu-id="49fa0-146">选择所在的国家/地区，然后选择“**Azure 订阅**”。</span><span class="sxs-lookup"><span data-stu-id="49fa0-146">Select your country or region, and then choose **Azure subscription**.</span></span>
    2. <span data-ttu-id="49fa0-p109">输入您的个人信息。输入可以与您取得联系的电话号码，并指定是要接收短信还是要接听来电，以作核实用途。</span><span class="sxs-lookup"><span data-stu-id="49fa0-p109">Enter your personal information. For verification purposes, enter a telephone number at which you can be reached, and specify whether you want to be sent a text message or called.</span></span>
    3. <span data-ttu-id="49fa0-149">在收到验证代码后，请输入此代码，然后选择“**验证代码**”。</span><span class="sxs-lookup"><span data-stu-id="49fa0-149">When you receive your verification code, enter it and choose **Verify code**.</span></span>
    4. <span data-ttu-id="49fa0-150">输入付款信息，检查协议，然后选择“**注册**”。</span><span class="sxs-lookup"><span data-stu-id="49fa0-150">Enter payment information, check the agreement, and select **Sign up**.</span></span>
        
        <span data-ttu-id="49fa0-151">你的信用卡将不会被扣费。</span><span class="sxs-lookup"><span data-stu-id="49fa0-151">Your credit card will not be charged.</span></span>
        
        <span data-ttu-id="49fa0-152">创建 Azure 订阅时不要关闭或刷新浏览器。</span><span class="sxs-lookup"><span data-stu-id="49fa0-152">Do not close or refresh your browser while your Azure subscription is being created.</span></span>
            
4. <span data-ttu-id="49fa0-153">创建 Azure 订阅后，请选择“**门户**”。</span><span class="sxs-lookup"><span data-stu-id="49fa0-153">When your Azure subscription is created, choose  **Portal**.</span></span>
        
5. <span data-ttu-id="49fa0-p110">此时，系统会显示 Azure 教程。你可以查看此教程，也可以选择“**X**”将它关闭。</span><span class="sxs-lookup"><span data-stu-id="49fa0-p110">The Azure Tour appears. You can view it, or choose  **X** to close it.</span></span>
        
    <span data-ttu-id="49fa0-p111">你现在应该可以在 Azure 订阅中看到所有项目。它列出了包含 Office 365 租户名称的目录。</span><span class="sxs-lookup"><span data-stu-id="49fa0-p111">You should now see all items in your Azure subscription. It lists a directory with the name of your Office 365 tenant.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="49fa0-158">另请参阅</span><span class="sxs-lookup"><span data-stu-id="49fa0-158">See also</span></span>
- [<span data-ttu-id="49fa0-159">在 Azure AD 中注册应用程序的基础知识</span><span class="sxs-lookup"><span data-stu-id="49fa0-159">Basics of Registering an Application in Azure AD</span></span>](https://azure.microsoft.com/zh-CN/documentation/articles/active-directory-authentication-scenarios/#basics-of-registering-an-application-in-azure-ad)
- [<span data-ttu-id="49fa0-160">在 Azure AD 中添加、更新或删除应用程序</span><span class="sxs-lookup"><span data-stu-id="49fa0-160">Add, update, or remove an application in Azure AD</span></span>](https://azure.microsoft.com/zh-CN/documentation/articles/active-directory-integrating-applications/)
