---
title: userPfxIntendedPurpose 枚举类型
description: 用户 PFX 证书的预期目的支持的值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ae43071956b3be505f5aaf98e1cf709cf8afa6c1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49300939"
---
# <a name="userpfxintendedpurpose-enum-type"></a><span data-ttu-id="f657c-103">userPfxIntendedPurpose 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f657c-103">userPfxIntendedPurpose enum type</span></span>

<span data-ttu-id="f657c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f657c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f657c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f657c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f657c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f657c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f657c-107">用户 PFX 证书的预期目的支持的值。</span><span class="sxs-lookup"><span data-stu-id="f657c-107">Supported values for the intended purpose of a user PFX certificate.</span></span>

## <a name="members"></a><span data-ttu-id="f657c-108">成员</span><span class="sxs-lookup"><span data-stu-id="f657c-108">Members</span></span>
|<span data-ttu-id="f657c-109">成员</span><span class="sxs-lookup"><span data-stu-id="f657c-109">Member</span></span>|<span data-ttu-id="f657c-110">值</span><span class="sxs-lookup"><span data-stu-id="f657c-110">Value</span></span>|<span data-ttu-id="f657c-111">Description</span><span class="sxs-lookup"><span data-stu-id="f657c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f657c-112">取消</span><span class="sxs-lookup"><span data-stu-id="f657c-112">unassigned</span></span>|<span data-ttu-id="f657c-113">0</span><span class="sxs-lookup"><span data-stu-id="f657c-113">0</span></span>|<span data-ttu-id="f657c-114">未分配角色/用法。</span><span class="sxs-lookup"><span data-stu-id="f657c-114">No roles/usages assigned.</span></span>|
|<span data-ttu-id="f657c-115">smimeEncryption</span><span class="sxs-lookup"><span data-stu-id="f657c-115">smimeEncryption</span></span>|<span data-ttu-id="f657c-116">1</span><span class="sxs-lookup"><span data-stu-id="f657c-116">1</span></span>|<span data-ttu-id="f657c-117">对 S/MIME 加密有效。</span><span class="sxs-lookup"><span data-stu-id="f657c-117">Valid for S/MIME encryption.</span></span>|
|<span data-ttu-id="f657c-118">smimeSigning</span><span class="sxs-lookup"><span data-stu-id="f657c-118">smimeSigning</span></span>|<span data-ttu-id="f657c-119">双面</span><span class="sxs-lookup"><span data-stu-id="f657c-119">2</span></span>|<span data-ttu-id="f657c-120">对 S/MIME 签名有效。</span><span class="sxs-lookup"><span data-stu-id="f657c-120">Valid for S/MIME signing.</span></span>|
|<span data-ttu-id="f657c-121">vpn</span><span class="sxs-lookup"><span data-stu-id="f657c-121">vpn</span></span>|<span data-ttu-id="f657c-122">4 </span><span class="sxs-lookup"><span data-stu-id="f657c-122">4</span></span>|<span data-ttu-id="f657c-123">在 VPN 中使用时有效。</span><span class="sxs-lookup"><span data-stu-id="f657c-123">Valid for use in VPN.</span></span>|
|<span data-ttu-id="f657c-124">wifi</span><span class="sxs-lookup"><span data-stu-id="f657c-124">wifi</span></span>|<span data-ttu-id="f657c-125">8 </span><span class="sxs-lookup"><span data-stu-id="f657c-125">8</span></span>|<span data-ttu-id="f657c-126">在 WiFi 中使用时有效。</span><span class="sxs-lookup"><span data-stu-id="f657c-126">Valid for use in WiFi.</span></span>|




