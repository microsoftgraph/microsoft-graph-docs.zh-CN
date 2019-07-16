---
title: userPfxIntendedPurpose 枚举类型
description: 用户 PFX 证书的预期目的支持的值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1790b1d1835d19cacb7e3b32262ce06be4daa378
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739279"
---
# <a name="userpfxintendedpurpose-enum-type"></a><span data-ttu-id="a3704-103">userPfxIntendedPurpose 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a3704-103">userPfxIntendedPurpose enum type</span></span>

> <span data-ttu-id="a3704-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a3704-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3704-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a3704-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3704-106">用户 PFX 证书的预期目的支持的值。</span><span class="sxs-lookup"><span data-stu-id="a3704-106">Supported values for the intended purpose of a user PFX certificate.</span></span>

## <a name="members"></a><span data-ttu-id="a3704-107">成员</span><span class="sxs-lookup"><span data-stu-id="a3704-107">Members</span></span>
|<span data-ttu-id="a3704-108">成员</span><span class="sxs-lookup"><span data-stu-id="a3704-108">Member</span></span>|<span data-ttu-id="a3704-109">值</span><span class="sxs-lookup"><span data-stu-id="a3704-109">Value</span></span>|<span data-ttu-id="a3704-110">说明</span><span class="sxs-lookup"><span data-stu-id="a3704-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3704-111">取消</span><span class="sxs-lookup"><span data-stu-id="a3704-111">unassigned</span></span>|<span data-ttu-id="a3704-112">0</span><span class="sxs-lookup"><span data-stu-id="a3704-112">0</span></span>|<span data-ttu-id="a3704-113">未分配角色/用法。</span><span class="sxs-lookup"><span data-stu-id="a3704-113">No roles/usages assigned.</span></span>|
|<span data-ttu-id="a3704-114">smimeEncryption</span><span class="sxs-lookup"><span data-stu-id="a3704-114">smimeEncryption</span></span>|<span data-ttu-id="a3704-115">1</span><span class="sxs-lookup"><span data-stu-id="a3704-115">1</span></span>|<span data-ttu-id="a3704-116">对 S/MIME 加密有效。</span><span class="sxs-lookup"><span data-stu-id="a3704-116">Valid for S/MIME encryption.</span></span>|
|<span data-ttu-id="a3704-117">smimeSigning</span><span class="sxs-lookup"><span data-stu-id="a3704-117">smimeSigning</span></span>|<span data-ttu-id="a3704-118">双面</span><span class="sxs-lookup"><span data-stu-id="a3704-118">2</span></span>|<span data-ttu-id="a3704-119">对 S/MIME 签名有效。</span><span class="sxs-lookup"><span data-stu-id="a3704-119">Valid for S/MIME signing.</span></span>|
|<span data-ttu-id="a3704-120">vpn</span><span class="sxs-lookup"><span data-stu-id="a3704-120">vpn</span></span>|<span data-ttu-id="a3704-121">4</span><span class="sxs-lookup"><span data-stu-id="a3704-121">4</span></span>|<span data-ttu-id="a3704-122">在 VPN 中使用时有效。</span><span class="sxs-lookup"><span data-stu-id="a3704-122">Valid for use in VPN.</span></span>|
|<span data-ttu-id="a3704-123">wifi</span><span class="sxs-lookup"><span data-stu-id="a3704-123">wifi</span></span>|<span data-ttu-id="a3704-124">utf-8</span><span class="sxs-lookup"><span data-stu-id="a3704-124">8</span></span>|<span data-ttu-id="a3704-125">在 WiFi 中使用时有效。</span><span class="sxs-lookup"><span data-stu-id="a3704-125">Valid for use in WiFi.</span></span>|





