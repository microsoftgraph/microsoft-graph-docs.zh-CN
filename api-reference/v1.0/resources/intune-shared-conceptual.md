---
title: 共享资源Microsoft Intune
description: 这些终结点在多个 Microsoft Graph API 中用于 Intune 工作流。  使用给定资源所需的意图、目的和权限因特定工作流和基础调用的上下文而异。  此外，某些方法、属性和操作仅受特定工作流支持。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: cc5cbf0f96d3c9199ecd9b622d9724ec10dd472e
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732371"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="55f42-105">共享资源Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="55f42-105">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="55f42-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55f42-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55f42-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户 [正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="55f42-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="55f42-108">这些终结点在多个 Microsoft Graph API 中用于 Intune 工作流。</span><span class="sxs-lookup"><span data-stu-id="55f42-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="55f42-109">使用给定资源所需的意图、目的和权限因特定工作流和基础调用的上下文而异。</span><span class="sxs-lookup"><span data-stu-id="55f42-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="55f42-110">此外，某些方法、属性和操作仅受特定工作流支持。</span><span class="sxs-lookup"><span data-stu-id="55f42-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="55f42-111">Intune Graph之间共享以下资源：</span><span class="sxs-lookup"><span data-stu-id="55f42-111">The following Graph resources are shared between Intune workflows:</span></span>  

- [<span data-ttu-id="55f42-112">所有设备分配目标</span><span class="sxs-lookup"><span data-stu-id="55f42-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="55f42-113">所有许可的用户分配目标</span><span class="sxs-lookup"><span data-stu-id="55f42-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="55f42-114">符合性状态</span><span class="sxs-lookup"><span data-stu-id="55f42-114">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="55f42-115">设备和应用管理分配目标</span><span class="sxs-lookup"><span data-stu-id="55f42-115">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="55f42-116">设备应用管理</span><span class="sxs-lookup"><span data-stu-id="55f42-116">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="55f42-117">设备类别</span><span class="sxs-lookup"><span data-stu-id="55f42-117">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="55f42-118">设备管理</span><span class="sxs-lookup"><span data-stu-id="55f42-118">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="55f42-119">排除组分配目标</span><span class="sxs-lookup"><span data-stu-id="55f42-119">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="55f42-120">组分配目标</span><span class="sxs-lookup"><span data-stu-id="55f42-120">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="55f42-121">安装意图</span><span class="sxs-lookup"><span data-stu-id="55f42-121">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="55f42-122">MIME 内容</span><span class="sxs-lookup"><span data-stu-id="55f42-122">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="55f42-123">报告</span><span class="sxs-lookup"><span data-stu-id="55f42-123">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="55f42-124">报表根目录</span><span class="sxs-lookup"><span data-stu-id="55f42-124">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="55f42-125">保存的 UI 状态生成选项</span><span class="sxs-lookup"><span data-stu-id="55f42-125">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="55f42-126">URI</span><span class="sxs-lookup"><span data-stu-id="55f42-126">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="55f42-127">用户</span><span class="sxs-lookup"><span data-stu-id="55f42-127">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="55f42-128">VPP 令牌帐户类型</span><span class="sxs-lookup"><span data-stu-id="55f42-128">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)






