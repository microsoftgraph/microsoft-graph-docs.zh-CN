---
title: win32LobAppRegistryDetectionType 枚举类型
description: 包含所有支持的注册表数据检测类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 188f206e42b55e0c2cc2f8b6ed831f19a4b2052a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411083"
---
# <a name="win32lobappregistrydetectiontype-enum-type"></a><span data-ttu-id="80027-103">win32LobAppRegistryDetectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="80027-103">win32LobAppRegistryDetectionType enum type</span></span>

> <span data-ttu-id="80027-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="80027-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="80027-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="80027-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80027-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="80027-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80027-107">包含所有支持的注册表数据检测类型。</span><span class="sxs-lookup"><span data-stu-id="80027-107">Contains all supported registry data detection type.</span></span>

## <a name="members"></a><span data-ttu-id="80027-108">成员</span><span class="sxs-lookup"><span data-stu-id="80027-108">Members</span></span>
|<span data-ttu-id="80027-109">成员</span><span class="sxs-lookup"><span data-stu-id="80027-109">Member</span></span>|<span data-ttu-id="80027-110">值</span><span class="sxs-lookup"><span data-stu-id="80027-110">Value</span></span>|<span data-ttu-id="80027-111">说明</span><span class="sxs-lookup"><span data-stu-id="80027-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80027-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="80027-112">notConfigured</span></span>|<span data-ttu-id="80027-113">0</span><span class="sxs-lookup"><span data-stu-id="80027-113">0</span></span>|<span data-ttu-id="80027-114">未配置。</span><span class="sxs-lookup"><span data-stu-id="80027-114">Not configured.</span></span>|
|<span data-ttu-id="80027-115">存在</span><span class="sxs-lookup"><span data-stu-id="80027-115">exists</span></span>|<span data-ttu-id="80027-116">1</span><span class="sxs-lookup"><span data-stu-id="80027-116">1</span></span>|<span data-ttu-id="80027-117">指定的注册表项或值存在。</span><span class="sxs-lookup"><span data-stu-id="80027-117">The specified registry key or value exists.</span></span>|
|<span data-ttu-id="80027-118">doesNotExist</span><span class="sxs-lookup"><span data-stu-id="80027-118">doesNotExist</span></span>|<span data-ttu-id="80027-119">2</span><span class="sxs-lookup"><span data-stu-id="80027-119">2</span></span>|<span data-ttu-id="80027-120">指定的注册表项的值不存在。</span><span class="sxs-lookup"><span data-stu-id="80027-120">The specified registry key or value does not exist.</span></span>|
|<span data-ttu-id="80027-121">string</span><span class="sxs-lookup"><span data-stu-id="80027-121">string</span></span>|<span data-ttu-id="80027-122">3</span><span class="sxs-lookup"><span data-stu-id="80027-122">3</span></span>|<span data-ttu-id="80027-123">字符串值类型。</span><span class="sxs-lookup"><span data-stu-id="80027-123">String value type.</span></span>|
|<span data-ttu-id="80027-124">integer</span><span class="sxs-lookup"><span data-stu-id="80027-124">integer</span></span>|<span data-ttu-id="80027-125">4</span><span class="sxs-lookup"><span data-stu-id="80027-125">4</span></span>|<span data-ttu-id="80027-126">整数值类型。</span><span class="sxs-lookup"><span data-stu-id="80027-126">Integer value type.</span></span>|
|<span data-ttu-id="80027-127">version</span><span class="sxs-lookup"><span data-stu-id="80027-127">version</span></span>|<span data-ttu-id="80027-128">5</span><span class="sxs-lookup"><span data-stu-id="80027-128">5</span></span>|<span data-ttu-id="80027-129">版本值类型。</span><span class="sxs-lookup"><span data-stu-id="80027-129">Version value type.</span></span>|




