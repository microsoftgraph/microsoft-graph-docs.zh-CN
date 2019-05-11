---
title: mobileAppPublishingState 枚举类型
description: 指示应用程序的发布状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ce69b2a2743496714fdb2697cec7e37a1efbaf19
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949918"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="542df-103">mobileAppPublishingState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="542df-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="542df-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="542df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="542df-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="542df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="542df-106">指示应用程序的发布状态。</span><span class="sxs-lookup"><span data-stu-id="542df-106">Indicates the publishing state of an app.</span></span>

## <a name="members"></a><span data-ttu-id="542df-107">成员</span><span class="sxs-lookup"><span data-stu-id="542df-107">Members</span></span>
|<span data-ttu-id="542df-108">成员</span><span class="sxs-lookup"><span data-stu-id="542df-108">Member</span></span>|<span data-ttu-id="542df-109">值</span><span class="sxs-lookup"><span data-stu-id="542df-109">Value</span></span>|<span data-ttu-id="542df-110">说明</span><span class="sxs-lookup"><span data-stu-id="542df-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="542df-111">notPublished</span><span class="sxs-lookup"><span data-stu-id="542df-111">notPublished</span></span>|<span data-ttu-id="542df-112">0</span><span class="sxs-lookup"><span data-stu-id="542df-112">0</span></span>|<span data-ttu-id="542df-113">应用尚未发布。</span><span class="sxs-lookup"><span data-stu-id="542df-113">The app is not yet published.</span></span>|
|<span data-ttu-id="542df-114">处理</span><span class="sxs-lookup"><span data-stu-id="542df-114">processing</span></span>|<span data-ttu-id="542df-115">1</span><span class="sxs-lookup"><span data-stu-id="542df-115">1</span></span>|<span data-ttu-id="542df-116">应用程序正在等待服务端处理。</span><span class="sxs-lookup"><span data-stu-id="542df-116">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="542df-117">发布</span><span class="sxs-lookup"><span data-stu-id="542df-117">published</span></span>|<span data-ttu-id="542df-118">双面</span><span class="sxs-lookup"><span data-stu-id="542df-118">2</span></span>|<span data-ttu-id="542df-119">应用程序已发布。</span><span class="sxs-lookup"><span data-stu-id="542df-119">The app is published.</span></span>|




