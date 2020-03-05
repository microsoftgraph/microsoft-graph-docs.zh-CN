---
title: userPfxIntendedPurpose 枚举类型
description: 用户 PFX 证书的预期目的支持的值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 00418943b8f10888f4517879907ad0bddfac47cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527584"
---
# <a name="userpfxintendedpurpose-enum-type"></a><span data-ttu-id="ca26c-103">userPfxIntendedPurpose 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ca26c-103">userPfxIntendedPurpose enum type</span></span>

<span data-ttu-id="ca26c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ca26c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca26c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ca26c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca26c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca26c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca26c-107">用户 PFX 证书的预期目的支持的值。</span><span class="sxs-lookup"><span data-stu-id="ca26c-107">Supported values for the intended purpose of a user PFX certificate.</span></span>

## <a name="members"></a><span data-ttu-id="ca26c-108">成员</span><span class="sxs-lookup"><span data-stu-id="ca26c-108">Members</span></span>
|<span data-ttu-id="ca26c-109">成员</span><span class="sxs-lookup"><span data-stu-id="ca26c-109">Member</span></span>|<span data-ttu-id="ca26c-110">值</span><span class="sxs-lookup"><span data-stu-id="ca26c-110">Value</span></span>|<span data-ttu-id="ca26c-111">说明</span><span class="sxs-lookup"><span data-stu-id="ca26c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca26c-112">取消</span><span class="sxs-lookup"><span data-stu-id="ca26c-112">unassigned</span></span>|<span data-ttu-id="ca26c-113">0</span><span class="sxs-lookup"><span data-stu-id="ca26c-113">0</span></span>|<span data-ttu-id="ca26c-114">未分配角色/用法。</span><span class="sxs-lookup"><span data-stu-id="ca26c-114">No roles/usages assigned.</span></span>|
|<span data-ttu-id="ca26c-115">smimeEncryption</span><span class="sxs-lookup"><span data-stu-id="ca26c-115">smimeEncryption</span></span>|<span data-ttu-id="ca26c-116">1 </span><span class="sxs-lookup"><span data-stu-id="ca26c-116">1</span></span>|<span data-ttu-id="ca26c-117">对 S/MIME 加密有效。</span><span class="sxs-lookup"><span data-stu-id="ca26c-117">Valid for S/MIME encryption.</span></span>|
|<span data-ttu-id="ca26c-118">smimeSigning</span><span class="sxs-lookup"><span data-stu-id="ca26c-118">smimeSigning</span></span>|<span data-ttu-id="ca26c-119">2 </span><span class="sxs-lookup"><span data-stu-id="ca26c-119">2</span></span>|<span data-ttu-id="ca26c-120">对 S/MIME 签名有效。</span><span class="sxs-lookup"><span data-stu-id="ca26c-120">Valid for S/MIME signing.</span></span>|
|<span data-ttu-id="ca26c-121">vpn</span><span class="sxs-lookup"><span data-stu-id="ca26c-121">vpn</span></span>|<span data-ttu-id="ca26c-122">4 </span><span class="sxs-lookup"><span data-stu-id="ca26c-122">4</span></span>|<span data-ttu-id="ca26c-123">在 VPN 中使用时有效。</span><span class="sxs-lookup"><span data-stu-id="ca26c-123">Valid for use in VPN.</span></span>|
|<span data-ttu-id="ca26c-124">wifi</span><span class="sxs-lookup"><span data-stu-id="ca26c-124">wifi</span></span>|<span data-ttu-id="ca26c-125">8 </span><span class="sxs-lookup"><span data-stu-id="ca26c-125">8</span></span>|<span data-ttu-id="ca26c-126">在 WiFi 中使用时有效。</span><span class="sxs-lookup"><span data-stu-id="ca26c-126">Valid for use in WiFi.</span></span>|



