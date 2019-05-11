---
title: firewallPreSharedKeyEncodingMethodType 枚举类型
description: FirewallPreSharedKeyEncodingMethod 的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 052eb026b7668f9159d1a091c32b229b1e1bf04d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946621"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="779a0-103">firewallPreSharedKeyEncodingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="779a0-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="779a0-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="779a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="779a0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="779a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="779a0-106">FirewallPreSharedKeyEncodingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="779a0-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="779a0-107">成员</span><span class="sxs-lookup"><span data-stu-id="779a0-107">Members</span></span>
|<span data-ttu-id="779a0-108">成员</span><span class="sxs-lookup"><span data-stu-id="779a0-108">Member</span></span>|<span data-ttu-id="779a0-109">值</span><span class="sxs-lookup"><span data-stu-id="779a0-109">Value</span></span>|<span data-ttu-id="779a0-110">说明</span><span class="sxs-lookup"><span data-stu-id="779a0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="779a0-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="779a0-111">deviceDefault</span></span>|<span data-ttu-id="779a0-112">0</span><span class="sxs-lookup"><span data-stu-id="779a0-112">0</span></span>|<span data-ttu-id="779a0-113">没有由 Intune 配置的值, 请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="779a0-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="779a0-114">无</span><span class="sxs-lookup"><span data-stu-id="779a0-114">none</span></span>|<span data-ttu-id="779a0-115">1</span><span class="sxs-lookup"><span data-stu-id="779a0-115">1</span></span>|<span data-ttu-id="779a0-116">未对预共享密钥进行编码。</span><span class="sxs-lookup"><span data-stu-id="779a0-116">Preshared key is not encoded.</span></span> <span data-ttu-id="779a0-117">相反, 它将保留为其宽字符格式</span><span class="sxs-lookup"><span data-stu-id="779a0-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="779a0-118">utF8</span><span class="sxs-lookup"><span data-stu-id="779a0-118">utF8</span></span>|<span data-ttu-id="779a0-119">双面</span><span class="sxs-lookup"><span data-stu-id="779a0-119">2</span></span>|<span data-ttu-id="779a0-120">使用 UTF-8 对预共享密钥进行编码</span><span class="sxs-lookup"><span data-stu-id="779a0-120">Encode the preshared key using UTF-8</span></span>|




