---
title: certificateRevocationStatus 枚举类型
description: 证书吊销状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 373cb6247a695a5912d02d4fb1a353c40aeac581
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421968"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="2c9f6-103">certificateRevocationStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2c9f6-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="2c9f6-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="2c9f6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2c9f6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2c9f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2c9f6-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2c9f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c9f6-107">证书吊销状态。</span><span class="sxs-lookup"><span data-stu-id="2c9f6-107">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="2c9f6-108">成员</span><span class="sxs-lookup"><span data-stu-id="2c9f6-108">Members</span></span>
|<span data-ttu-id="2c9f6-109">成员</span><span class="sxs-lookup"><span data-stu-id="2c9f6-109">Member</span></span>|<span data-ttu-id="2c9f6-110">值</span><span class="sxs-lookup"><span data-stu-id="2c9f6-110">Value</span></span>|<span data-ttu-id="2c9f6-111">说明</span><span class="sxs-lookup"><span data-stu-id="2c9f6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c9f6-112">无</span><span class="sxs-lookup"><span data-stu-id="2c9f6-112">none</span></span>|<span data-ttu-id="2c9f6-113">0</span><span class="sxs-lookup"><span data-stu-id="2c9f6-113">0</span></span>|<span data-ttu-id="2c9f6-114">未被吊销。</span><span class="sxs-lookup"><span data-stu-id="2c9f6-114">Not revoked.</span></span>|
|<span data-ttu-id="2c9f6-115">挂起</span><span class="sxs-lookup"><span data-stu-id="2c9f6-115">pending</span></span>|<span data-ttu-id="2c9f6-116">1</span><span class="sxs-lookup"><span data-stu-id="2c9f6-116">1</span></span>|<span data-ttu-id="2c9f6-117">待处理的吊销。</span><span class="sxs-lookup"><span data-stu-id="2c9f6-117">Revocation pending.</span></span>|
|<span data-ttu-id="2c9f6-118">颁发</span><span class="sxs-lookup"><span data-stu-id="2c9f6-118">issued</span></span>|<span data-ttu-id="2c9f6-119">2</span><span class="sxs-lookup"><span data-stu-id="2c9f6-119">2</span></span>|<span data-ttu-id="2c9f6-120">吊销发出命令。</span><span class="sxs-lookup"><span data-stu-id="2c9f6-120">Revocation command issued.</span></span>|
|<span data-ttu-id="2c9f6-121">failed</span><span class="sxs-lookup"><span data-stu-id="2c9f6-121">failed</span></span>|<span data-ttu-id="2c9f6-122">3</span><span class="sxs-lookup"><span data-stu-id="2c9f6-122">3</span></span>|<span data-ttu-id="2c9f6-123">吊销失败。</span><span class="sxs-lookup"><span data-stu-id="2c9f6-123">Revocation failed.</span></span>|
|<span data-ttu-id="2c9f6-124">吊销</span><span class="sxs-lookup"><span data-stu-id="2c9f6-124">revoked</span></span>|<span data-ttu-id="2c9f6-125">4</span><span class="sxs-lookup"><span data-stu-id="2c9f6-125">4</span></span>|<span data-ttu-id="2c9f6-126">吊销。</span><span class="sxs-lookup"><span data-stu-id="2c9f6-126">Revoked.</span></span>|




