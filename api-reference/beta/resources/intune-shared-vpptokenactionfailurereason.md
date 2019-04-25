---
title: vppTokenActionFailureReason 枚举类型
description: Apple volume purchase program 令牌操作失败的可能原因类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9adb896d384be99496c016ef3bd39b02ff1a28e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548255"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="6846b-103">vppTokenActionFailureReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6846b-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="6846b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6846b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6846b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6846b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6846b-106">Apple volume purchase program 令牌操作失败的可能原因类型。</span><span class="sxs-lookup"><span data-stu-id="6846b-106">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="6846b-107">成员</span><span class="sxs-lookup"><span data-stu-id="6846b-107">Members</span></span>
|<span data-ttu-id="6846b-108">成员</span><span class="sxs-lookup"><span data-stu-id="6846b-108">Member</span></span>|<span data-ttu-id="6846b-109">值</span><span class="sxs-lookup"><span data-stu-id="6846b-109">Value</span></span>|<span data-ttu-id="6846b-110">说明</span><span class="sxs-lookup"><span data-stu-id="6846b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6846b-111">无</span><span class="sxs-lookup"><span data-stu-id="6846b-111">none</span></span>|<span data-ttu-id="6846b-112">0</span><span class="sxs-lookup"><span data-stu-id="6846b-112">0</span></span>|<span data-ttu-id="6846b-113">无。</span><span class="sxs-lookup"><span data-stu-id="6846b-113">None.</span></span>|
|<span data-ttu-id="6846b-114">appleFailure</span><span class="sxs-lookup"><span data-stu-id="6846b-114">appleFailure</span></span>|<span data-ttu-id="6846b-115">1</span><span class="sxs-lookup"><span data-stu-id="6846b-115">1</span></span>|<span data-ttu-id="6846b-116">Apple 的服务上出现错误。</span><span class="sxs-lookup"><span data-stu-id="6846b-116">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="6846b-117">internalError</span><span class="sxs-lookup"><span data-stu-id="6846b-117">internalError</span></span>|<span data-ttu-id="6846b-118">2 </span><span class="sxs-lookup"><span data-stu-id="6846b-118">2</span></span>|<span data-ttu-id="6846b-119">有一个内部错误。</span><span class="sxs-lookup"><span data-stu-id="6846b-119">There was an internal error.</span></span>|
|<span data-ttu-id="6846b-120">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="6846b-120">expiredVppToken</span></span>|<span data-ttu-id="6846b-121">3 </span><span class="sxs-lookup"><span data-stu-id="6846b-121">3</span></span>|<span data-ttu-id="6846b-122">由于 Apple volume purchase program 令牌已过期, 因此出现错误。</span><span class="sxs-lookup"><span data-stu-id="6846b-122">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="6846b-123">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="6846b-123">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="6846b-124">4 </span><span class="sxs-lookup"><span data-stu-id="6846b-124">4</span></span>|<span data-ttu-id="6846b-125">由于 Apple volume purchase program 推送通知证书已过期, 因此出现错误。</span><span class="sxs-lookup"><span data-stu-id="6846b-125">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|





