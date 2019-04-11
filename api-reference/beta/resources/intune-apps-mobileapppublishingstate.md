---
title: mobileAppPublishingState 枚举类型
description: 指示应用程序的发布状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5e644264c1e72092be16063156708b45364b5097
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782749"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="4c9a9-103">mobileAppPublishingState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4c9a9-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="4c9a9-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4c9a9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c9a9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4c9a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c9a9-106">指示应用程序的发布状态。</span><span class="sxs-lookup"><span data-stu-id="4c9a9-106">Indicates the publishing state of an app.</span></span>

## <a name="members"></a><span data-ttu-id="4c9a9-107">成员</span><span class="sxs-lookup"><span data-stu-id="4c9a9-107">Members</span></span>
|<span data-ttu-id="4c9a9-108">成员</span><span class="sxs-lookup"><span data-stu-id="4c9a9-108">Member</span></span>|<span data-ttu-id="4c9a9-109">值</span><span class="sxs-lookup"><span data-stu-id="4c9a9-109">Value</span></span>|<span data-ttu-id="4c9a9-110">说明</span><span class="sxs-lookup"><span data-stu-id="4c9a9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c9a9-111">notPublished</span><span class="sxs-lookup"><span data-stu-id="4c9a9-111">notPublished</span></span>|<span data-ttu-id="4c9a9-112">0</span><span class="sxs-lookup"><span data-stu-id="4c9a9-112">0</span></span>|<span data-ttu-id="4c9a9-113">应用尚未发布。</span><span class="sxs-lookup"><span data-stu-id="4c9a9-113">The app is not yet published.</span></span>|
|<span data-ttu-id="4c9a9-114">处理</span><span class="sxs-lookup"><span data-stu-id="4c9a9-114">processing</span></span>|<span data-ttu-id="4c9a9-115">1</span><span class="sxs-lookup"><span data-stu-id="4c9a9-115">1</span></span>|<span data-ttu-id="4c9a9-116">应用程序正在等待服务端处理。</span><span class="sxs-lookup"><span data-stu-id="4c9a9-116">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="4c9a9-117">发布</span><span class="sxs-lookup"><span data-stu-id="4c9a9-117">published</span></span>|<span data-ttu-id="4c9a9-118">双面</span><span class="sxs-lookup"><span data-stu-id="4c9a9-118">2</span></span>|<span data-ttu-id="4c9a9-119">应用程序已发布。</span><span class="sxs-lookup"><span data-stu-id="4c9a9-119">The app is published.</span></span>|





