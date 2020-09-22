---
title: mobileAppPublishingState 枚举类型
description: 指示应用程序的发布状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: dcd6d0ee560d660f3c9d355a3417971dce6b4ffe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094328"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="36512-103">mobileAppPublishingState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="36512-103">mobileAppPublishingState enum type</span></span>

<span data-ttu-id="36512-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36512-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36512-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="36512-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36512-106">指示应用程序的发布状态。</span><span class="sxs-lookup"><span data-stu-id="36512-106">Indicates the publishing state of an app.</span></span>

## <a name="members"></a><span data-ttu-id="36512-107">成员</span><span class="sxs-lookup"><span data-stu-id="36512-107">Members</span></span>
|<span data-ttu-id="36512-108">成员</span><span class="sxs-lookup"><span data-stu-id="36512-108">Member</span></span>|<span data-ttu-id="36512-109">值</span><span class="sxs-lookup"><span data-stu-id="36512-109">Value</span></span>|<span data-ttu-id="36512-110">说明</span><span class="sxs-lookup"><span data-stu-id="36512-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36512-111">notPublished</span><span class="sxs-lookup"><span data-stu-id="36512-111">notPublished</span></span>|<span data-ttu-id="36512-112">0</span><span class="sxs-lookup"><span data-stu-id="36512-112">0</span></span>|<span data-ttu-id="36512-113">应用尚未发布。</span><span class="sxs-lookup"><span data-stu-id="36512-113">The app is not yet published.</span></span>|
|<span data-ttu-id="36512-114">处理</span><span class="sxs-lookup"><span data-stu-id="36512-114">processing</span></span>|<span data-ttu-id="36512-115">1 </span><span class="sxs-lookup"><span data-stu-id="36512-115">1</span></span>|<span data-ttu-id="36512-116">应用程序正在等待服务端处理。</span><span class="sxs-lookup"><span data-stu-id="36512-116">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="36512-117">发布</span><span class="sxs-lookup"><span data-stu-id="36512-117">published</span></span>|<span data-ttu-id="36512-118">2 </span><span class="sxs-lookup"><span data-stu-id="36512-118">2</span></span>|<span data-ttu-id="36512-119">应用程序已发布。</span><span class="sxs-lookup"><span data-stu-id="36512-119">The app is published.</span></span>|









