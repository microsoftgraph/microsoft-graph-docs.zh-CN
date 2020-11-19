---
title: vppTokenActionFailureReason 枚举类型
description: Apple Volume Purchase Program 令牌操作失败的可能原因类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ad2151be841133b7fbbbd6bc858e9ecdf3e611d6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49271679"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="abf8f-103">vppTokenActionFailureReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="abf8f-103">vppTokenActionFailureReason enum type</span></span>

<span data-ttu-id="abf8f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abf8f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="abf8f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="abf8f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abf8f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="abf8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abf8f-107">Apple Volume Purchase Program 令牌操作失败的可能原因类型。</span><span class="sxs-lookup"><span data-stu-id="abf8f-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="abf8f-108">成员</span><span class="sxs-lookup"><span data-stu-id="abf8f-108">Members</span></span>
|<span data-ttu-id="abf8f-109">成员</span><span class="sxs-lookup"><span data-stu-id="abf8f-109">Member</span></span>|<span data-ttu-id="abf8f-110">值</span><span class="sxs-lookup"><span data-stu-id="abf8f-110">Value</span></span>|<span data-ttu-id="abf8f-111">说明</span><span class="sxs-lookup"><span data-stu-id="abf8f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abf8f-112">无</span><span class="sxs-lookup"><span data-stu-id="abf8f-112">none</span></span>|<span data-ttu-id="abf8f-113">0</span><span class="sxs-lookup"><span data-stu-id="abf8f-113">0</span></span>|<span data-ttu-id="abf8f-114">无。</span><span class="sxs-lookup"><span data-stu-id="abf8f-114">None.</span></span>|
|<span data-ttu-id="abf8f-115">appleFailure</span><span class="sxs-lookup"><span data-stu-id="abf8f-115">appleFailure</span></span>|<span data-ttu-id="abf8f-116">1</span><span class="sxs-lookup"><span data-stu-id="abf8f-116">1</span></span>|<span data-ttu-id="abf8f-117">Apple 的服务上出现错误。</span><span class="sxs-lookup"><span data-stu-id="abf8f-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="abf8f-118">internalError</span><span class="sxs-lookup"><span data-stu-id="abf8f-118">internalError</span></span>|<span data-ttu-id="abf8f-119">双面</span><span class="sxs-lookup"><span data-stu-id="abf8f-119">2</span></span>|<span data-ttu-id="abf8f-120">有一个内部错误。</span><span class="sxs-lookup"><span data-stu-id="abf8f-120">There was an internal error.</span></span>|
|<span data-ttu-id="abf8f-121">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="abf8f-121">expiredVppToken</span></span>|<span data-ttu-id="abf8f-122">第三章</span><span class="sxs-lookup"><span data-stu-id="abf8f-122">3</span></span>|<span data-ttu-id="abf8f-123">由于 Apple Volume Purchase Program 令牌已过期，因此出现错误。</span><span class="sxs-lookup"><span data-stu-id="abf8f-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="abf8f-124">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="abf8f-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="abf8f-125">4 </span><span class="sxs-lookup"><span data-stu-id="abf8f-125">4</span></span>|<span data-ttu-id="abf8f-126">由于 Apple Volume Purchase Program 推送通知证书已过期，因此出现错误。</span><span class="sxs-lookup"><span data-stu-id="abf8f-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|




