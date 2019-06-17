---
title: vppTokenActionFailureReason 枚举类型
description: Apple Volume Purchase Program 令牌操作失败的可能原因类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0f8aacb6fc6f95b8c8085a78ed2851b16622357
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990986"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="da974-103">vppTokenActionFailureReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="da974-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="da974-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="da974-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da974-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da974-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da974-106">Apple Volume Purchase Program 令牌操作失败的可能原因类型。</span><span class="sxs-lookup"><span data-stu-id="da974-106">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="da974-107">成员</span><span class="sxs-lookup"><span data-stu-id="da974-107">Members</span></span>
|<span data-ttu-id="da974-108">成员</span><span class="sxs-lookup"><span data-stu-id="da974-108">Member</span></span>|<span data-ttu-id="da974-109">值</span><span class="sxs-lookup"><span data-stu-id="da974-109">Value</span></span>|<span data-ttu-id="da974-110">说明</span><span class="sxs-lookup"><span data-stu-id="da974-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da974-111">无</span><span class="sxs-lookup"><span data-stu-id="da974-111">none</span></span>|<span data-ttu-id="da974-112">0</span><span class="sxs-lookup"><span data-stu-id="da974-112">0</span></span>|<span data-ttu-id="da974-113">无。</span><span class="sxs-lookup"><span data-stu-id="da974-113">None.</span></span>|
|<span data-ttu-id="da974-114">appleFailure</span><span class="sxs-lookup"><span data-stu-id="da974-114">appleFailure</span></span>|<span data-ttu-id="da974-115">1</span><span class="sxs-lookup"><span data-stu-id="da974-115">1</span></span>|<span data-ttu-id="da974-116">Apple 的服务上出现错误。</span><span class="sxs-lookup"><span data-stu-id="da974-116">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="da974-117">internalError</span><span class="sxs-lookup"><span data-stu-id="da974-117">internalError</span></span>|<span data-ttu-id="da974-118">双面</span><span class="sxs-lookup"><span data-stu-id="da974-118">2</span></span>|<span data-ttu-id="da974-119">有一个内部错误。</span><span class="sxs-lookup"><span data-stu-id="da974-119">There was an internal error.</span></span>|
|<span data-ttu-id="da974-120">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="da974-120">expiredVppToken</span></span>|<span data-ttu-id="da974-121">第三章</span><span class="sxs-lookup"><span data-stu-id="da974-121">3</span></span>|<span data-ttu-id="da974-122">由于 Apple Volume Purchase Program 令牌已过期, 因此出现错误。</span><span class="sxs-lookup"><span data-stu-id="da974-122">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="da974-123">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="da974-123">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="da974-124">4</span><span class="sxs-lookup"><span data-stu-id="da974-124">4</span></span>|<span data-ttu-id="da974-125">由于 Apple Volume Purchase Program 推送通知证书已过期, 因此出现错误。</span><span class="sxs-lookup"><span data-stu-id="da974-125">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|





