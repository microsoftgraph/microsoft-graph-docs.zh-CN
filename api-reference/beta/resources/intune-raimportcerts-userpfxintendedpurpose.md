---
title: userPfxIntendedPurpose 枚举类型
description: 用户 PFX 证书的预期目的支持的值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8db764032db2d15a93441d98cb0169ebc0316ca7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726316"
---
# <a name="userpfxintendedpurpose-enum-type"></a><span data-ttu-id="3b922-103">userPfxIntendedPurpose 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3b922-103">userPfxIntendedPurpose enum type</span></span>

<span data-ttu-id="3b922-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b922-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b922-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3b922-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b922-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3b922-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b922-107">用户 PFX 证书的预期目的支持的值。</span><span class="sxs-lookup"><span data-stu-id="3b922-107">Supported values for the intended purpose of a user PFX certificate.</span></span>

## <a name="members"></a><span data-ttu-id="3b922-108">成员</span><span class="sxs-lookup"><span data-stu-id="3b922-108">Members</span></span>
|<span data-ttu-id="3b922-109">成员</span><span class="sxs-lookup"><span data-stu-id="3b922-109">Member</span></span>|<span data-ttu-id="3b922-110">值</span><span class="sxs-lookup"><span data-stu-id="3b922-110">Value</span></span>|<span data-ttu-id="3b922-111">说明</span><span class="sxs-lookup"><span data-stu-id="3b922-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b922-112">取消</span><span class="sxs-lookup"><span data-stu-id="3b922-112">unassigned</span></span>|<span data-ttu-id="3b922-113">0</span><span class="sxs-lookup"><span data-stu-id="3b922-113">0</span></span>|<span data-ttu-id="3b922-114">未分配角色/用法。</span><span class="sxs-lookup"><span data-stu-id="3b922-114">No roles/usages assigned.</span></span>|
|<span data-ttu-id="3b922-115">smimeEncryption</span><span class="sxs-lookup"><span data-stu-id="3b922-115">smimeEncryption</span></span>|<span data-ttu-id="3b922-116">1</span><span class="sxs-lookup"><span data-stu-id="3b922-116">1</span></span>|<span data-ttu-id="3b922-117">对 S/MIME 加密有效。</span><span class="sxs-lookup"><span data-stu-id="3b922-117">Valid for S/MIME encryption.</span></span>|
|<span data-ttu-id="3b922-118">smimeSigning</span><span class="sxs-lookup"><span data-stu-id="3b922-118">smimeSigning</span></span>|<span data-ttu-id="3b922-119">双面</span><span class="sxs-lookup"><span data-stu-id="3b922-119">2</span></span>|<span data-ttu-id="3b922-120">对 S/MIME 签名有效。</span><span class="sxs-lookup"><span data-stu-id="3b922-120">Valid for S/MIME signing.</span></span>|
|<span data-ttu-id="3b922-121">vpn</span><span class="sxs-lookup"><span data-stu-id="3b922-121">vpn</span></span>|<span data-ttu-id="3b922-122">4 </span><span class="sxs-lookup"><span data-stu-id="3b922-122">4</span></span>|<span data-ttu-id="3b922-123">在 VPN 中使用时有效。</span><span class="sxs-lookup"><span data-stu-id="3b922-123">Valid for use in VPN.</span></span>|
|<span data-ttu-id="3b922-124">wifi</span><span class="sxs-lookup"><span data-stu-id="3b922-124">wifi</span></span>|<span data-ttu-id="3b922-125">8 </span><span class="sxs-lookup"><span data-stu-id="3b922-125">8</span></span>|<span data-ttu-id="3b922-126">在 WiFi 中使用时有效。</span><span class="sxs-lookup"><span data-stu-id="3b922-126">Valid for use in WiFi.</span></span>|





