---
title: Microsoft Graph 数据连接（预览）入门
description: 'Office 365 管理员必须先执行两个操作，以便管理员能够通过 Privileged Access Management (PAM) 控制数据移动，之后你才可以使用 Microsoft Graph 数据连接。 '
author: ajacks-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: f7426147908a2ded298bee065c05afffc182cd4b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526117"
---
# <a name="get-started-with-microsoft-graph-data-connect-preview"></a><span data-ttu-id="77c8d-103">Microsoft Graph 数据连接（预览）入门</span><span class="sxs-lookup"><span data-stu-id="77c8d-103">Get started with Microsoft Graph data connect (preview)</span></span>

<span data-ttu-id="77c8d-104">Office 365 管理员必须先执行两个操作，以便管理员能够通过 Privileged Access Management (PAM) 控制数据移动，之后你才可以使用 Microsoft Graph 数据连接。</span><span class="sxs-lookup"><span data-stu-id="77c8d-104">Before you can use Microsoft Graph data connect, an Office 365 administrator must take two actions, both of which enable the ability for the admin to control data movement through Privileged Access Management (PAM).</span></span> 

1. <span data-ttu-id="77c8d-105">通过 Microsoft 365 管理门户的“服务和加载项”页同意选择使用 Microsoft Graph 数据连接。\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="77c8d-105">Give consent to opt in to Microsoft Graph data connect through the Microsoft 365 Admin Portal, on the **Services & add-ins** page.</span></span> <span data-ttu-id="77c8d-106">这样即允许了对 Microsoft Azure 的数据移动请求（即保持对数据的完全控制，但允许 Azure 资源访问它）。</span><span class="sxs-lookup"><span data-stu-id="77c8d-106">This will allow data movement requests to Microsoft Azure (that is, keep full control over the data, but allow Azure resources to access it).</span></span> <span data-ttu-id="77c8d-107">在提供对特定管道的批准前，无法迁移任何数据。</span><span class="sxs-lookup"><span data-stu-id="77c8d-107">No data is transferred unless approval for a specific pipeline is provided later.</span></span>
2. <span data-ttu-id="77c8d-108">在 Office 365 订阅中设置审批者组。</span><span class="sxs-lookup"><span data-stu-id="77c8d-108">Set an approver group within the Office 365 subscription.</span></span> <span data-ttu-id="77c8d-109">确保审批者组不为空。</span><span class="sxs-lookup"><span data-stu-id="77c8d-109">Make sure that the approver group is not empty.</span></span> <span data-ttu-id="77c8d-110">仅此组中的用户可以批准数据移动请求。</span><span class="sxs-lookup"><span data-stu-id="77c8d-110">Only the users in the group can approve data movement requests.</span></span>

<span data-ttu-id="77c8d-111">可参阅 [Microsoft Graph 数据连接培训模块](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md)，来获取详细的分步说明。</span><span class="sxs-lookup"><span data-stu-id="77c8d-111">For detailed step-by-step instructions, see the [Microsoft Graph data connect training module](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="77c8d-112">后续步骤</span><span class="sxs-lookup"><span data-stu-id="77c8d-112">Next steps</span></span>

<span data-ttu-id="77c8d-113">恭喜！</span><span class="sxs-lookup"><span data-stu-id="77c8d-113">Congratulations!</span></span> <span data-ttu-id="77c8d-114">现在你即可开始使用 Azure 工具生成智能应用程序。</span><span class="sxs-lookup"><span data-stu-id="77c8d-114">You're now ready to start building intelligent applications with Azure tooling.</span></span> <span data-ttu-id="77c8d-115">可参阅 [Microsoft Graph 数据连接 GitHub 存储库](https://github.com/OfficeDev/MS-Graph-Data-Connect/wiki)来获取示例应用程序和更多文档。</span><span class="sxs-lookup"><span data-stu-id="77c8d-115">For a sample application and additional documentation, see the [Microsoft Graph data connect GitHub repo](https://github.com/OfficeDev/MS-Graph-Data-Connect/wiki).</span></span> 
