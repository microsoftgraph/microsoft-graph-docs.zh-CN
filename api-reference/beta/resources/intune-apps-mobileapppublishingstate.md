---
title: mobileAppPublishingState 枚举类型
description: 指示应用程序的发布状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 070140c004834ef878415e9e20d77d00cfb6c2d8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076356"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="16e90-103">mobileAppPublishingState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="16e90-103">mobileAppPublishingState enum type</span></span>

<span data-ttu-id="16e90-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16e90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16e90-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="16e90-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16e90-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="16e90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16e90-107">指示应用程序的发布状态。</span><span class="sxs-lookup"><span data-stu-id="16e90-107">Indicates the publishing state of an app.</span></span>

## <a name="members"></a><span data-ttu-id="16e90-108">成员</span><span class="sxs-lookup"><span data-stu-id="16e90-108">Members</span></span>
|<span data-ttu-id="16e90-109">成员</span><span class="sxs-lookup"><span data-stu-id="16e90-109">Member</span></span>|<span data-ttu-id="16e90-110">值</span><span class="sxs-lookup"><span data-stu-id="16e90-110">Value</span></span>|<span data-ttu-id="16e90-111">说明</span><span class="sxs-lookup"><span data-stu-id="16e90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16e90-112">notPublished</span><span class="sxs-lookup"><span data-stu-id="16e90-112">notPublished</span></span>|<span data-ttu-id="16e90-113">0</span><span class="sxs-lookup"><span data-stu-id="16e90-113">0</span></span>|<span data-ttu-id="16e90-114">应用尚未发布。</span><span class="sxs-lookup"><span data-stu-id="16e90-114">The app is not yet published.</span></span>|
|<span data-ttu-id="16e90-115">处理</span><span class="sxs-lookup"><span data-stu-id="16e90-115">processing</span></span>|<span data-ttu-id="16e90-116">1 </span><span class="sxs-lookup"><span data-stu-id="16e90-116">1</span></span>|<span data-ttu-id="16e90-117">应用程序正在等待服务端处理。</span><span class="sxs-lookup"><span data-stu-id="16e90-117">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="16e90-118">发布</span><span class="sxs-lookup"><span data-stu-id="16e90-118">published</span></span>|<span data-ttu-id="16e90-119">2 </span><span class="sxs-lookup"><span data-stu-id="16e90-119">2</span></span>|<span data-ttu-id="16e90-120">应用程序已发布。</span><span class="sxs-lookup"><span data-stu-id="16e90-120">The app is published.</span></span>|






