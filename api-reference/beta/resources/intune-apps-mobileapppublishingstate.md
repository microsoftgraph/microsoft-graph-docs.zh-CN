---
title: mobileAppPublishingState 枚举类型
description: 指示应用程序的发布状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 34e2d06701513e4070384307f49f5dfd0d2b50de
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991854"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="64dc2-103">mobileAppPublishingState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="64dc2-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="64dc2-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="64dc2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64dc2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="64dc2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64dc2-106">指示应用程序的发布状态。</span><span class="sxs-lookup"><span data-stu-id="64dc2-106">Indicates the publishing state of an app.</span></span>

## <a name="members"></a><span data-ttu-id="64dc2-107">成员</span><span class="sxs-lookup"><span data-stu-id="64dc2-107">Members</span></span>
|<span data-ttu-id="64dc2-108">成员</span><span class="sxs-lookup"><span data-stu-id="64dc2-108">Member</span></span>|<span data-ttu-id="64dc2-109">值</span><span class="sxs-lookup"><span data-stu-id="64dc2-109">Value</span></span>|<span data-ttu-id="64dc2-110">说明</span><span class="sxs-lookup"><span data-stu-id="64dc2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64dc2-111">notPublished</span><span class="sxs-lookup"><span data-stu-id="64dc2-111">notPublished</span></span>|<span data-ttu-id="64dc2-112">0</span><span class="sxs-lookup"><span data-stu-id="64dc2-112">0</span></span>|<span data-ttu-id="64dc2-113">应用尚未发布。</span><span class="sxs-lookup"><span data-stu-id="64dc2-113">The app is not yet published.</span></span>|
|<span data-ttu-id="64dc2-114">处理</span><span class="sxs-lookup"><span data-stu-id="64dc2-114">processing</span></span>|<span data-ttu-id="64dc2-115">1</span><span class="sxs-lookup"><span data-stu-id="64dc2-115">1</span></span>|<span data-ttu-id="64dc2-116">应用程序正在等待服务端处理。</span><span class="sxs-lookup"><span data-stu-id="64dc2-116">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="64dc2-117">发布</span><span class="sxs-lookup"><span data-stu-id="64dc2-117">published</span></span>|<span data-ttu-id="64dc2-118">双面</span><span class="sxs-lookup"><span data-stu-id="64dc2-118">2</span></span>|<span data-ttu-id="64dc2-119">应用程序已发布。</span><span class="sxs-lookup"><span data-stu-id="64dc2-119">The app is published.</span></span>|





