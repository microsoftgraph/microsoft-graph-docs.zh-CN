---
title: edgeKioskModeRestrictionType 枚举类型
description: 根据展台模式指定 Microsoft Edge 设置的限制方式。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a5fecf749b7aacef1c9eb0c465889f37e080ddb3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199117"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="f4101-103">edgeKioskModeRestrictionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f4101-103">edgeKioskModeRestrictionType enum type</span></span>

<span data-ttu-id="f4101-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4101-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4101-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4101-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4101-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4101-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4101-107">根据展台模式指定 Microsoft Edge 设置的限制方式。</span><span class="sxs-lookup"><span data-stu-id="f4101-107">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="f4101-108">成员</span><span class="sxs-lookup"><span data-stu-id="f4101-108">Members</span></span>
|<span data-ttu-id="f4101-109">成员</span><span class="sxs-lookup"><span data-stu-id="f4101-109">Member</span></span>|<span data-ttu-id="f4101-110">值</span><span class="sxs-lookup"><span data-stu-id="f4101-110">Value</span></span>|<span data-ttu-id="f4101-111">说明</span><span class="sxs-lookup"><span data-stu-id="f4101-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4101-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f4101-112">notConfigured</span></span>|<span data-ttu-id="f4101-113">0</span><span class="sxs-lookup"><span data-stu-id="f4101-113">0</span></span>|<span data-ttu-id="f4101-114">未 (不受限制的) 配置。</span><span class="sxs-lookup"><span data-stu-id="f4101-114">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="f4101-115">digitalSignage</span><span class="sxs-lookup"><span data-stu-id="f4101-115">digitalSignage</span></span>|<span data-ttu-id="f4101-116">1</span><span class="sxs-lookup"><span data-stu-id="f4101-116">1</span></span>|<span data-ttu-id="f4101-117">单应用模式中的交互/数字告示。</span><span class="sxs-lookup"><span data-stu-id="f4101-117">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="f4101-118">normalMode</span><span class="sxs-lookup"><span data-stu-id="f4101-118">normalMode</span></span>|<span data-ttu-id="f4101-119">双面</span><span class="sxs-lookup"><span data-stu-id="f4101-119">2</span></span>|<span data-ttu-id="f4101-120">正常模式 (Microsoft Edge) 的完整版本。</span><span class="sxs-lookup"><span data-stu-id="f4101-120">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="f4101-121">publicBrowsingSingleApp</span><span class="sxs-lookup"><span data-stu-id="f4101-121">publicBrowsingSingleApp</span></span>|<span data-ttu-id="f4101-122">第三章</span><span class="sxs-lookup"><span data-stu-id="f4101-122">3</span></span>|<span data-ttu-id="f4101-123">单应用模式中的公共浏览。</span><span class="sxs-lookup"><span data-stu-id="f4101-123">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="f4101-124">publicBrowsingMultiApp</span><span class="sxs-lookup"><span data-stu-id="f4101-124">publicBrowsingMultiApp</span></span>|<span data-ttu-id="f4101-125">4 </span><span class="sxs-lookup"><span data-stu-id="f4101-125">4</span></span>|<span data-ttu-id="f4101-126">在多应用模式下，公共浏览 (inPrivate) 。</span><span class="sxs-lookup"><span data-stu-id="f4101-126">Public browsing (inPrivate) in multi-app mode.</span></span>|




