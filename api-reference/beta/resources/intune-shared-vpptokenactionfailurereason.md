---
title: vppTokenActionFailureReason 枚举类型
description: 可能的 Apple 卷购买计划令牌操作失败的原因的类型。
ms.openlocfilehash: 0fece0417a5585540f15e3f8a8631fd30eaa414e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044081"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="df787-103">vppTokenActionFailureReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="df787-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="df787-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="df787-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df787-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="df787-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df787-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="df787-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df787-107">可能的 Apple 卷购买计划令牌操作失败的原因的类型。</span><span class="sxs-lookup"><span data-stu-id="df787-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>
## <a name="members"></a><span data-ttu-id="df787-108">成员</span><span class="sxs-lookup"><span data-stu-id="df787-108">Members</span></span>
|<span data-ttu-id="df787-109">成员</span><span class="sxs-lookup"><span data-stu-id="df787-109">Member</span></span>|<span data-ttu-id="df787-110">值</span><span class="sxs-lookup"><span data-stu-id="df787-110">Value</span></span>|<span data-ttu-id="df787-111">说明</span><span class="sxs-lookup"><span data-stu-id="df787-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df787-112">无</span><span class="sxs-lookup"><span data-stu-id="df787-112">none</span></span>|<span data-ttu-id="df787-113">0</span><span class="sxs-lookup"><span data-stu-id="df787-113">0</span></span>|<span data-ttu-id="df787-114">无。</span><span class="sxs-lookup"><span data-stu-id="df787-114">None.</span></span>|
|<span data-ttu-id="df787-115">appleFailure</span><span class="sxs-lookup"><span data-stu-id="df787-115">appleFailure</span></span>|<span data-ttu-id="df787-116">1</span><span class="sxs-lookup"><span data-stu-id="df787-116">1</span></span>|<span data-ttu-id="df787-117">在 Apple 的服务时出错。</span><span class="sxs-lookup"><span data-stu-id="df787-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="df787-118">internalError</span><span class="sxs-lookup"><span data-stu-id="df787-118">internalError</span></span>|<span data-ttu-id="df787-119">2</span><span class="sxs-lookup"><span data-stu-id="df787-119">2</span></span>|<span data-ttu-id="df787-120">存在内部错误。</span><span class="sxs-lookup"><span data-stu-id="df787-120">There was an internal error.</span></span>|
|<span data-ttu-id="df787-121">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="df787-121">expiredVppToken</span></span>|<span data-ttu-id="df787-122">3</span><span class="sxs-lookup"><span data-stu-id="df787-122">3</span></span>|<span data-ttu-id="df787-123">因为 Apple 卷购买计划令牌已过期时出错。</span><span class="sxs-lookup"><span data-stu-id="df787-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="df787-124">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="df787-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="df787-125">4</span><span class="sxs-lookup"><span data-stu-id="df787-125">4</span></span>|<span data-ttu-id="df787-126">由于 Apple 卷购买程序推送通知证书过期时出错。</span><span class="sxs-lookup"><span data-stu-id="df787-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|





