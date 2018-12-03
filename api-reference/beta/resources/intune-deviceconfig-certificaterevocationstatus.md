---
title: certificateRevocationStatus 枚举类型
description: 证书吊销状态。
ms.openlocfilehash: 5fb80b85cb6fe65e20439f8a3242b6bc74b30184
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042938"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="d485c-103">certificateRevocationStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d485c-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="d485c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d485c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d485c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d485c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d485c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d485c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d485c-107">证书吊销状态。</span><span class="sxs-lookup"><span data-stu-id="d485c-107">Certificate Revocation Status.</span></span>
## <a name="members"></a><span data-ttu-id="d485c-108">成员</span><span class="sxs-lookup"><span data-stu-id="d485c-108">Members</span></span>
|<span data-ttu-id="d485c-109">成员</span><span class="sxs-lookup"><span data-stu-id="d485c-109">Member</span></span>|<span data-ttu-id="d485c-110">值</span><span class="sxs-lookup"><span data-stu-id="d485c-110">Value</span></span>|<span data-ttu-id="d485c-111">说明</span><span class="sxs-lookup"><span data-stu-id="d485c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d485c-112">无</span><span class="sxs-lookup"><span data-stu-id="d485c-112">none</span></span>|<span data-ttu-id="d485c-113">0</span><span class="sxs-lookup"><span data-stu-id="d485c-113">0</span></span>|<span data-ttu-id="d485c-114">未被吊销。</span><span class="sxs-lookup"><span data-stu-id="d485c-114">Not revoked.</span></span>|
|<span data-ttu-id="d485c-115">挂起</span><span class="sxs-lookup"><span data-stu-id="d485c-115">pending</span></span>|<span data-ttu-id="d485c-116">1</span><span class="sxs-lookup"><span data-stu-id="d485c-116">1</span></span>|<span data-ttu-id="d485c-117">待处理的吊销。</span><span class="sxs-lookup"><span data-stu-id="d485c-117">Revocation pending.</span></span>|
|<span data-ttu-id="d485c-118">颁发</span><span class="sxs-lookup"><span data-stu-id="d485c-118">issued</span></span>|<span data-ttu-id="d485c-119">2</span><span class="sxs-lookup"><span data-stu-id="d485c-119">2</span></span>|<span data-ttu-id="d485c-120">吊销发出命令。</span><span class="sxs-lookup"><span data-stu-id="d485c-120">Revocation command issued.</span></span>|
|<span data-ttu-id="d485c-121">failed</span><span class="sxs-lookup"><span data-stu-id="d485c-121">failed</span></span>|<span data-ttu-id="d485c-122">3</span><span class="sxs-lookup"><span data-stu-id="d485c-122">3</span></span>|<span data-ttu-id="d485c-123">吊销失败。</span><span class="sxs-lookup"><span data-stu-id="d485c-123">Revocation failed.</span></span>|
|<span data-ttu-id="d485c-124">吊销</span><span class="sxs-lookup"><span data-stu-id="d485c-124">revoked</span></span>|<span data-ttu-id="d485c-125">4</span><span class="sxs-lookup"><span data-stu-id="d485c-125">4</span></span>|<span data-ttu-id="d485c-126">吊销。</span><span class="sxs-lookup"><span data-stu-id="d485c-126">Revoked.</span></span>|





