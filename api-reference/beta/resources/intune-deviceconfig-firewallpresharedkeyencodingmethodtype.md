---
title: firewallPreSharedKeyEncodingMethodType 枚举类型
description: FirewallPreSharedKeyEncodingMethod 的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ddd167d69674c0e32c184aa0f68bd7698331ee3c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004295"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="cda0b-103">firewallPreSharedKeyEncodingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cda0b-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="cda0b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cda0b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cda0b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cda0b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cda0b-106">FirewallPreSharedKeyEncodingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="cda0b-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="cda0b-107">成员</span><span class="sxs-lookup"><span data-stu-id="cda0b-107">Members</span></span>
|<span data-ttu-id="cda0b-108">成员</span><span class="sxs-lookup"><span data-stu-id="cda0b-108">Member</span></span>|<span data-ttu-id="cda0b-109">值</span><span class="sxs-lookup"><span data-stu-id="cda0b-109">Value</span></span>|<span data-ttu-id="cda0b-110">说明</span><span class="sxs-lookup"><span data-stu-id="cda0b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cda0b-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="cda0b-111">deviceDefault</span></span>|<span data-ttu-id="cda0b-112">0</span><span class="sxs-lookup"><span data-stu-id="cda0b-112">0</span></span>|<span data-ttu-id="cda0b-113">没有由 Intune 配置的值, 请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="cda0b-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="cda0b-114">无</span><span class="sxs-lookup"><span data-stu-id="cda0b-114">none</span></span>|<span data-ttu-id="cda0b-115">1</span><span class="sxs-lookup"><span data-stu-id="cda0b-115">1</span></span>|<span data-ttu-id="cda0b-116">未对预共享密钥进行编码。</span><span class="sxs-lookup"><span data-stu-id="cda0b-116">Preshared key is not encoded.</span></span> <span data-ttu-id="cda0b-117">相反, 它将保留为其宽字符格式</span><span class="sxs-lookup"><span data-stu-id="cda0b-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="cda0b-118">utF8</span><span class="sxs-lookup"><span data-stu-id="cda0b-118">utF8</span></span>|<span data-ttu-id="cda0b-119">双面</span><span class="sxs-lookup"><span data-stu-id="cda0b-119">2</span></span>|<span data-ttu-id="cda0b-120">使用 UTF-8 对预共享密钥进行编码</span><span class="sxs-lookup"><span data-stu-id="cda0b-120">Encode the preshared key using UTF-8</span></span>|





