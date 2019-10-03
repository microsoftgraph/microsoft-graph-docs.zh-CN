---
title: Microsoft Intune 中的共享资源
description: 这些终结点在多个 Microsoft Graph API for Intune 工作流中使用。  使用给定资源所需的意向、目的和权限因特定工作流和基础调用的上下文而异。  此外，特定工作流仅支持某些方法、属性和操作。
localization_priority: Normal
author: davidmu1
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 2fdf99fe8116213c418eae62a7297112ed5871f0
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368286"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="ce25a-105">Microsoft Intune 中的共享资源</span><span class="sxs-lookup"><span data-stu-id="ce25a-105">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="ce25a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ce25a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="ce25a-107">这些终结点在多个 Microsoft Graph API for Intune 工作流中使用。</span><span class="sxs-lookup"><span data-stu-id="ce25a-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="ce25a-108">使用给定资源所需的意向、目的和权限因特定工作流和基础调用的上下文而异。</span><span class="sxs-lookup"><span data-stu-id="ce25a-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="ce25a-109">此外，特定工作流仅支持某些方法、属性和操作。</span><span class="sxs-lookup"><span data-stu-id="ce25a-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="ce25a-110">以下关系图资源在 Intune 工作流之间共享：</span><span class="sxs-lookup"><span data-stu-id="ce25a-110">The following Graph resources are shared between Intune workflows:</span></span>  

- [<span data-ttu-id="ce25a-111">所有设备分配目标</span><span class="sxs-lookup"><span data-stu-id="ce25a-111">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="ce25a-112">所有许可的用户分配目标</span><span class="sxs-lookup"><span data-stu-id="ce25a-112">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="ce25a-113">符合性状态</span><span class="sxs-lookup"><span data-stu-id="ce25a-113">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="ce25a-114">设备和应用管理分配目标</span><span class="sxs-lookup"><span data-stu-id="ce25a-114">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="ce25a-115">设备应用管理</span><span class="sxs-lookup"><span data-stu-id="ce25a-115">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="ce25a-116">设备类别</span><span class="sxs-lookup"><span data-stu-id="ce25a-116">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="ce25a-117">设备管理</span><span class="sxs-lookup"><span data-stu-id="ce25a-117">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="ce25a-118">排除组分配目标</span><span class="sxs-lookup"><span data-stu-id="ce25a-118">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="ce25a-119">组分配目标</span><span class="sxs-lookup"><span data-stu-id="ce25a-119">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="ce25a-120">安装意图</span><span class="sxs-lookup"><span data-stu-id="ce25a-120">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="ce25a-121">MIME 内容</span><span class="sxs-lookup"><span data-stu-id="ce25a-121">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="ce25a-122">Report</span><span class="sxs-lookup"><span data-stu-id="ce25a-122">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="ce25a-123">报表根目录</span><span class="sxs-lookup"><span data-stu-id="ce25a-123">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="ce25a-124">保存的 UI 状态生成选项</span><span class="sxs-lookup"><span data-stu-id="ce25a-124">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="ce25a-125">URI</span><span class="sxs-lookup"><span data-stu-id="ce25a-125">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="ce25a-126">用户</span><span class="sxs-lookup"><span data-stu-id="ce25a-126">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="ce25a-127">VPP 令牌帐户类型</span><span class="sxs-lookup"><span data-stu-id="ce25a-127">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)

