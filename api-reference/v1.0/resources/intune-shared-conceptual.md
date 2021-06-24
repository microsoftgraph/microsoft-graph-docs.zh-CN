---
title: 共享资源Microsoft Intune
description: 这些终结点在多个 Microsoft Graph API 中用于 Intune 工作流。  使用给定资源所需的意图、目的和权限因特定工作流和基础调用的上下文而异。  此外，某些方法、属性和操作仅受特定工作流支持。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 0af56b1ec3014fdee14dc4b70d3c14208321581a
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108885"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="108d8-105">共享资源Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="108d8-105">Shared resources in Microsoft Intune</span></span>

<span data-ttu-id="108d8-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="108d8-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="108d8-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户 [正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="108d8-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="108d8-108">这些终结点在多个 Microsoft Graph API 中用于 Intune 工作流。</span><span class="sxs-lookup"><span data-stu-id="108d8-108">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="108d8-109">使用给定资源所需的意图、目的和权限因特定工作流和基础调用的上下文而异。</span><span class="sxs-lookup"><span data-stu-id="108d8-109">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="108d8-110">此外，某些方法、属性和操作仅受特定工作流支持。</span><span class="sxs-lookup"><span data-stu-id="108d8-110">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="108d8-111">Intune Graph之间共享以下资源：</span><span class="sxs-lookup"><span data-stu-id="108d8-111">The following Graph resources are shared between Intune workflows:</span></span>  

- [<span data-ttu-id="108d8-112">所有设备分配目标</span><span class="sxs-lookup"><span data-stu-id="108d8-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="108d8-113">所有许可的用户分配目标</span><span class="sxs-lookup"><span data-stu-id="108d8-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="108d8-114">Android 企业始终使用 VPN 程序包类型</span><span class="sxs-lookup"><span data-stu-id="108d8-114">Android enterprise always on VPN package type</span></span>](intune-shared-androidenterprisealwaysonvpnpackagetype.md)
- [<span data-ttu-id="108d8-115">符合性状态</span><span class="sxs-lookup"><span data-stu-id="108d8-115">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="108d8-116">配置管理器集合分配目标</span><span class="sxs-lookup"><span data-stu-id="108d8-116">Configuration manager collection assignment target</span></span>](intune-shared-configurationmanagercollectionassignmenttarget.md)
- [<span data-ttu-id="108d8-117">设备和应用管理分配目标</span><span class="sxs-lookup"><span data-stu-id="108d8-117">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="108d8-118">排除组分配目标</span><span class="sxs-lookup"><span data-stu-id="108d8-118">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="108d8-119">组分配目标</span><span class="sxs-lookup"><span data-stu-id="108d8-119">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="108d8-120">安装意图</span><span class="sxs-lookup"><span data-stu-id="108d8-120">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="108d8-121">MIME 内容</span><span class="sxs-lookup"><span data-stu-id="108d8-121">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="108d8-122">保存的 UI 状态生成选项</span><span class="sxs-lookup"><span data-stu-id="108d8-122">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="108d8-123">URI</span><span class="sxs-lookup"><span data-stu-id="108d8-123">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="108d8-124">VPP 令牌帐户类型</span><span class="sxs-lookup"><span data-stu-id="108d8-124">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)