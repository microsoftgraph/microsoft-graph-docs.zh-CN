---
title: 开始使用 Microsoft Graph 数据连接 （预览）
description: '您可以使用数据连接的 Microsoft Graph 之前，Office 365 管理员必须执行两个操作，这两种启用与控件数据移动到特权访问管理 (PAM) 管理的功能。 '
ms.openlocfilehash: eb21f0d850f64694514c0ecd82f03de687606a56
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091769"
---
# <a name="get-started-with-microsoft-graph-data-connect-preview"></a><span data-ttu-id="fa7a3-103">开始使用 Microsoft Graph 数据连接 （预览）</span><span class="sxs-lookup"><span data-stu-id="fa7a3-103">Get started with Microsoft Graph data connect (preview)</span></span>

<span data-ttu-id="fa7a3-104">您可以使用数据连接的 Microsoft Graph 之前，Office 365 管理员必须执行两个操作，这两种启用与控件数据移动到特权访问管理 (PAM) 管理的功能。</span><span class="sxs-lookup"><span data-stu-id="fa7a3-104">Before you can use Microsoft Graph data connect, an Office 365 administrator must take two actions, both of which enable the ability for the admin to control data movement through Privileged Access Management (PAM).</span></span> 

1. <span data-ttu-id="fa7a3-105">授予许可选择 Microsoft Graph 通过 Microsoft 365 管理门户中，在**服务和外接程序**页上的数据连接。</span><span class="sxs-lookup"><span data-stu-id="fa7a3-105">Give consent to opt in to Microsoft Graph data connect through the Microsoft 365 Admin Portal, on the **Services & add-ins** page.</span></span> <span data-ttu-id="fa7a3-106">这将使数据对 Microsoft Azure （即，保留完全控制数据，但允许 Azure 资源访问） 的移动请求。</span><span class="sxs-lookup"><span data-stu-id="fa7a3-106">This will allow data movement requests to Microsoft Azure (that is, keep full control over the data, but allow Azure resources to access it).</span></span> <span data-ttu-id="fa7a3-107">除非为特定管道审批提供更高版本，则会不传输任何数据。</span><span class="sxs-lookup"><span data-stu-id="fa7a3-107">No data is transferred unless approval for a specific pipeline is provided later.</span></span>
2. <span data-ttu-id="fa7a3-108">设置 Office 365 订阅中的审批者组。</span><span class="sxs-lookup"><span data-stu-id="fa7a3-108">Set an approver group within the Office 365 subscription.</span></span> <span data-ttu-id="fa7a3-109">请确保审批者组不为空。</span><span class="sxs-lookup"><span data-stu-id="fa7a3-109">Make sure that the approver group is not empty.</span></span> <span data-ttu-id="fa7a3-110">组中的用户可以审核数据的移动请求。</span><span class="sxs-lookup"><span data-stu-id="fa7a3-110">Only the users in the group can approve data movement requests.</span></span>

<span data-ttu-id="fa7a3-111">有关详细的分步说明，请参阅[Microsoft Graph 数据连接培训模块](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md)。</span><span class="sxs-lookup"><span data-stu-id="fa7a3-111">For detailed step-by-step instructions, see the [Microsoft Graph data connect training module](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="fa7a3-112">后续步骤</span><span class="sxs-lookup"><span data-stu-id="fa7a3-112">Next steps</span></span>

<span data-ttu-id="fa7a3-113">恭喜你!</span><span class="sxs-lookup"><span data-stu-id="fa7a3-113">Congratulations!</span></span> <span data-ttu-id="fa7a3-114">您现在已准备好开始构建使用 Azure 工具智能应用程序。</span><span class="sxs-lookup"><span data-stu-id="fa7a3-114">You're now ready to start building intelligent applications with Azure tooling.</span></span> <span data-ttu-id="fa7a3-115">示例应用程序和其他文档，请参阅[Microsoft Graph 数据连接 GitHub repo](https://github.com/OfficeDev/MS-Graph-Data-Connect/wiki)。</span><span class="sxs-lookup"><span data-stu-id="fa7a3-115">For a sample application and additional documentation, see the [Microsoft Graph data connect GitHub repo](https://github.com/OfficeDev/MS-Graph-Data-Connect/wiki).</span></span> 
