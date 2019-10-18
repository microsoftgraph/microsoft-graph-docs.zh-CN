---
title: Microsoft Graph 数据连接入门
description: 'Office 365 管理员必须先执行两个操作，以便管理员能够通过 Privileged Access Management (PAM) 控制数据移动，之后你才可以使用 Microsoft Graph 数据连接。 '
author: ajacks-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 0fda5a21b59a1f6abfeeca864ce0d299618c5fdd
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34537161"
---
# <a name="get-started-with-microsoft-graph-data-connect"></a><span data-ttu-id="66541-103">Microsoft Graph 数据连接入门</span><span class="sxs-lookup"><span data-stu-id="66541-103">Get started with Microsoft Graph data connect</span></span>

<span data-ttu-id="66541-104">Office 365 管理员必须先执行两个操作，以便管理员能够通过 Privileged Access Management (PAM) 控制数据移动，之后你才可以使用 Microsoft Graph 数据连接。</span><span class="sxs-lookup"><span data-stu-id="66541-104">Before you can use Microsoft Graph data connect, an Office 365 administrator must take two actions, both of which enable the ability for the admin to control data movement through Privileged Access Management (PAM).</span></span> 

1. <span data-ttu-id="66541-105">通过 Microsoft 365 管理门户的“服务和加载项”页同意选择使用 Microsoft Graph 数据连接。\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="66541-105">Give consent to opt in to Microsoft Graph data connect through the Microsoft 365 Admin Portal, on the **Services & add-ins** page.</span></span> <span data-ttu-id="66541-106">这样即允许了对 Microsoft Azure 的数据移动请求（即保持对数据的完全控制，但允许 Azure 资源访问它）。</span><span class="sxs-lookup"><span data-stu-id="66541-106">This will allow data movement requests to Microsoft Azure (that is, keep full control over the data, but allow Azure resources to access it).</span></span> <span data-ttu-id="66541-107">在提供对特定管道的批准前，无法迁移任何数据。</span><span class="sxs-lookup"><span data-stu-id="66541-107">No data is transferred unless approval for a specific pipeline is provided later.</span></span>
2. <span data-ttu-id="66541-108">在 Office 365 订阅中设置已启用邮件的安全组或通讯组列表。</span><span class="sxs-lookup"><span data-stu-id="66541-108">Set a mail-enabled security group or distribution list within the Office 365 subscription.</span></span> <span data-ttu-id="66541-109">确保审批者组不为空。</span><span class="sxs-lookup"><span data-stu-id="66541-109">Make sure that the approver group is not empty.</span></span> <span data-ttu-id="66541-110">仅此组中的用户可以批准数据移动请求。</span><span class="sxs-lookup"><span data-stu-id="66541-110">Only the users in the group can approve data movement requests.</span></span>

## <a name="next-steps"></a><span data-ttu-id="66541-111">后续步骤</span><span class="sxs-lookup"><span data-stu-id="66541-111">Next steps</span></span>

<span data-ttu-id="66541-112">恭喜！</span><span class="sxs-lookup"><span data-stu-id="66541-112">Congratulations!</span></span> <span data-ttu-id="66541-113">现在你即可开始使用 Azure 工具生成智能应用程序。</span><span class="sxs-lookup"><span data-stu-id="66541-113">You're now ready to start building intelligent applications with Azure tooling.</span></span> <span data-ttu-id="66541-114">可参阅 [Microsoft Graph 数据连接培训模块](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md)，来获取详细的分步说明。</span><span class="sxs-lookup"><span data-stu-id="66541-114">For detailed step-by-step instructions, see the [Microsoft Graph data connect training module](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md).</span></span> <span data-ttu-id="66541-115">要详细了解 Microsoft Graph 数据连接提供的功能，请参阅数据连接支持的[数据集、区域和接收器](data-connect-datasets.md)或[用户选择和筛选](data-connect-filtering.md)。</span><span class="sxs-lookup"><span data-stu-id="66541-115">For more information about the capabilities that Microsoft Graph data connect provides, see [datasets, regions, and sinks](data-connect-datasets.md) or [user selection and filtering](data-connect-filtering.md) that data connect supports.</span></span>
