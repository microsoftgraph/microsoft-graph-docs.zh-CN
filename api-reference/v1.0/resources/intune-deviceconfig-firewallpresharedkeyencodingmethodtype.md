---
title: firewallPreSharedKeyEncodingMethodType 枚举类型
description: FirewallPreSharedKeyEncodingMethod 的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 07ea8e7a3a5622446ab2c0126d21187f6d7ce3b9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359234"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="8eb59-103">firewallPreSharedKeyEncodingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8eb59-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="8eb59-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8eb59-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8eb59-105">FirewallPreSharedKeyEncodingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="8eb59-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="8eb59-106">成员</span><span class="sxs-lookup"><span data-stu-id="8eb59-106">Members</span></span>
|<span data-ttu-id="8eb59-107">成员</span><span class="sxs-lookup"><span data-stu-id="8eb59-107">Member</span></span>|<span data-ttu-id="8eb59-108">值</span><span class="sxs-lookup"><span data-stu-id="8eb59-108">Value</span></span>|<span data-ttu-id="8eb59-109">说明</span><span class="sxs-lookup"><span data-stu-id="8eb59-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8eb59-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="8eb59-110">deviceDefault</span></span>|<span data-ttu-id="8eb59-111">0</span><span class="sxs-lookup"><span data-stu-id="8eb59-111">0</span></span>|<span data-ttu-id="8eb59-112">没有由 Intune 配置的值，请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="8eb59-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="8eb59-113">无</span><span class="sxs-lookup"><span data-stu-id="8eb59-113">none</span></span>|<span data-ttu-id="8eb59-114">1</span><span class="sxs-lookup"><span data-stu-id="8eb59-114">1</span></span>|<span data-ttu-id="8eb59-115">未对预共享密钥进行编码。</span><span class="sxs-lookup"><span data-stu-id="8eb59-115">Preshared key is not encoded.</span></span> <span data-ttu-id="8eb59-116">相反，它将保留为其宽字符格式</span><span class="sxs-lookup"><span data-stu-id="8eb59-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="8eb59-117">utF8</span><span class="sxs-lookup"><span data-stu-id="8eb59-117">utF8</span></span>|<span data-ttu-id="8eb59-118">双面</span><span class="sxs-lookup"><span data-stu-id="8eb59-118">2</span></span>|<span data-ttu-id="8eb59-119">使用 UTF-8 对预共享密钥进行编码</span><span class="sxs-lookup"><span data-stu-id="8eb59-119">Encode the preshared key using UTF-8</span></span>|




