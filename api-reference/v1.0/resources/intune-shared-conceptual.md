---
title: Microsoft Intune 中的共享资源
description: 这些终结点在多个 Microsoft Graph API for Intune 工作流中使用。  使用给定资源所需的意向、目的和权限因特定工作流和基础调用的上下文而异。  此外，特定工作流仅支持某些方法、属性和操作。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 04ecd6062dfbcba3ff885e9734a6802440866725
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448292"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="ec89c-105">Microsoft Intune 中的共享资源</span><span class="sxs-lookup"><span data-stu-id="ec89c-105">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="ec89c-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec89c-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec89c-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ec89c-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="ec89c-108">这些终结点在多个 Microsoft Graph API for Intune 工作流中使用。</span><span class="sxs-lookup"><span data-stu-id="ec89c-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="ec89c-109">使用给定资源所需的意向、目的和权限因特定工作流和基础调用的上下文而异。</span><span class="sxs-lookup"><span data-stu-id="ec89c-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="ec89c-110">此外，特定工作流仅支持某些方法、属性和操作。</span><span class="sxs-lookup"><span data-stu-id="ec89c-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="ec89c-111">以下关系图资源在 Intune 工作流之间共享：</span><span class="sxs-lookup"><span data-stu-id="ec89c-111">The following Graph resources are shared between Intune workflows:</span></span>  

- [<span data-ttu-id="ec89c-112">所有设备分配目标</span><span class="sxs-lookup"><span data-stu-id="ec89c-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="ec89c-113">所有许可的用户分配目标</span><span class="sxs-lookup"><span data-stu-id="ec89c-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="ec89c-114">符合性状态</span><span class="sxs-lookup"><span data-stu-id="ec89c-114">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="ec89c-115">设备和应用管理分配目标</span><span class="sxs-lookup"><span data-stu-id="ec89c-115">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="ec89c-116">设备应用管理</span><span class="sxs-lookup"><span data-stu-id="ec89c-116">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="ec89c-117">设备类别</span><span class="sxs-lookup"><span data-stu-id="ec89c-117">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="ec89c-118">设备管理</span><span class="sxs-lookup"><span data-stu-id="ec89c-118">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="ec89c-119">排除组分配目标</span><span class="sxs-lookup"><span data-stu-id="ec89c-119">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="ec89c-120">组分配目标</span><span class="sxs-lookup"><span data-stu-id="ec89c-120">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="ec89c-121">安装意图</span><span class="sxs-lookup"><span data-stu-id="ec89c-121">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="ec89c-122">MIME 内容</span><span class="sxs-lookup"><span data-stu-id="ec89c-122">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="ec89c-123">Report</span><span class="sxs-lookup"><span data-stu-id="ec89c-123">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="ec89c-124">报表根目录</span><span class="sxs-lookup"><span data-stu-id="ec89c-124">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="ec89c-125">保存的 UI 状态生成选项</span><span class="sxs-lookup"><span data-stu-id="ec89c-125">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="ec89c-126">URI</span><span class="sxs-lookup"><span data-stu-id="ec89c-126">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="ec89c-127">用户</span><span class="sxs-lookup"><span data-stu-id="ec89c-127">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="ec89c-128">VPP 令牌帐户类型</span><span class="sxs-lookup"><span data-stu-id="ec89c-128">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)




