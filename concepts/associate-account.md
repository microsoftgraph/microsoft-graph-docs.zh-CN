---
title: 将 Office 365 帐户与 Azure AD 相关联以创建和管理应用
description: '若要使用 Microsoft Azure Active Directory (Azure AD) 验证应用，必须在 Azure AD 中注册应用。这也是存储 Office 365 用户帐户和应用信息的位置。必须有 Microsoft Azure 订阅，才能通过 Azure 门户管理 Azure AD。可以使用 Microsoft Azure 门户管理用户、角色和应用。 '
ms.openlocfilehash: 1a0935a88d985d8be72197c2652586bbbc19bd1d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091831"
---
# <a name="associate-your-office-365-account-with-azure-ad-to-create-and-manage-apps"></a>将 Office 365 帐户与 Azure AD 相关联以创建和管理应用

若要使用 Microsoft Azure Active Directory (Azure AD) 验证应用，必须在 Azure AD 中注册应用。这也是存储 Office 365 用户帐户和应用信息的位置。必须有 Microsoft Azure 订阅，才能通过 Azure 门户管理 Azure AD。可以使用 Microsoft Azure 门户管理用户、角色和应用。 

本文介绍了如何将 Office 365 帐户和 Azure AD 相关联，以创建和管理应用。

 >**注意：** 本文将 Azure AD 用作应用的身份验证提供程序。如果使用的是 Azure AD v2.0 终结点，则无需执行此步骤。有关详细信息，请参阅 [Microsoft Graph 的应用身份验证](auth-overview.md)。

## <a name="prerequisites"></a>先决条件

**Office 365 商业版帐户**

如果没有现成的 Office 365 商业版帐户，则可以：

- 注册上面列出的 [Office 365 商业版计划](https://products.office.com/en-us/business/compare-office-365-for-business-plans)，或
- [参加 Office 365 开发人员计划并获取为期 1 年的免费 Office 365 订阅](https://aka.ms/devprogramsignup)。

**Microsoft Azure 订阅** 

- 如果有现成的 Microsoft Azure 订阅，则可以将它与 Office 365 商业版订阅相关联。 

- 否则，您将需要新建一个 Azure 订阅，并将它与您的 Office 365 帐户相关联以便注册和管理应用。


<!---<a name="bk_AssociateExistingAzureSubscription"> </a>-->

## <a name="to-associate-an-existing-azure-subscription-with-your-office-365-account"></a>关联现有 Azure 订阅和 Office 365 帐户的具体步骤


1. 使用现有 Azure 凭据（例如，user@live.com 等 Microsoft ID）登录 [Microsoft Azure 门户](https://portal.azure.com)。
        
2. 依次选择“Active Directory”**** 节点、“目录”**** 选项卡和屏幕底部的“新建”****。 
     
4. 在“**新建**”菜单中，依次选择“**Active Directory**” > “**目录**” > “**自定义创建**”。
    
5. 在“**添加目录**”中，在“**目录**”下拉框中，选择“**使用现有目录**”。单击“**我已准备好注销**”，然后选中右下角的复选标记。 
    
    这样可以返回到 Azure 门户。
        
3. 使用 Office 365 帐户信息登录。 
    
    系统将提示是否要通过 Azure 使用目录。 
    
    >**重要说明：** 若要将 Office 365 帐户与 Azure AD 相关联，则需要具有全局管理员权限的 Office 365 商业版帐户。 
    
        
4. 依次选择“继续”**** 和“立即注销”****。
        
5. 关闭浏览器，然后重新打开[门户](https://manage.windowsazure.com)。否则，你将收到访问被拒绝错误。
    
        
6. 使用现有的 Azure 凭据（例如，诸如 user@live.com 之类的 Microsoft ID）重新登录。转到“**Active Directory**”节点，在“**目录**”下，应该会看到 Office 365 帐户被列出。
    

<!--<a name="bk_AssociateNewAzureSubscription"> </a>-->

## <a name="to-create-a-new-azure-subscription-and-associate-it-with-your-office-365-account"></a>若要新建 Azure 订阅并将它与 Office 365 帐户相关联


1. 登录 Office 365。在“**主页**”中，选择“**管理员**”图标，打开 Office 365 管理中心。
2. 在菜单页中，沿着页面左侧，向下滚动到“管理员”****，再选择“Azure AD”****。

    >**重要说明：** 若要打开 Office 365 管理中心，则需要具有全局管理员权限的 Office 365 商业版帐户。 
    
3. 新建一个订阅。
        
    如果使用 Office 365 的试用版，您将看到一条消息告诉您 Azure AD 仅限使用付费服务的客户使用。仍然可以免费创建 30 天试用 Azure 订阅，但需要执行几个额外的步骤：
    
    1. 选择所在的国家/地区，然后选择“**Azure 订阅**”。
    2. 输入您的个人信息。输入可以与您取得联系的电话号码，并指定是要接收短信还是要接听来电，以作核实用途。
    3. 在收到验证代码后，请输入此代码，然后选择“**验证代码**”。
    4. 输入付款信息，检查协议，然后选择“**注册**”。
        
        你的信用卡将不会被扣费。
        
        创建 Azure 订阅时不要关闭或刷新浏览器。
            
4. 创建 Azure 订阅后，请选择“**门户**”。
        
5. 此时，系统会显示 Azure 教程。你可以查看此教程，也可以选择“**X**”将它关闭。
        
    现在应该可以在 Azure 订阅中看到所有项。它列出了包含 Office 365 租户名称的目录。
    
## <a name="see-also"></a>另请参阅
- [在 Azure AD 中注册应用程序的基础知识](https://azure.microsoft.com/en-us/documentation/articles/active-directory-authentication-scenarios/#basics-of-registering-an-application-in-azure-ad)
- [在 Azure AD 中添加、更新或删除应用程序](https://azure.microsoft.com/en-us/documentation/articles/active-directory-integrating-applications/)