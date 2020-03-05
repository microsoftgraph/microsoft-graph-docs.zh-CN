---
title: firewallPreSharedKeyEncodingMethodType 枚举类型
description: FirewallPreSharedKeyEncodingMethod 的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0e2b5a3094ea0e5f351d67968254250156f98453
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526435"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="c7e0b-103">firewallPreSharedKeyEncodingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c7e0b-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

<span data-ttu-id="c7e0b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c7e0b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7e0b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c7e0b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7e0b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7e0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7e0b-107">FirewallPreSharedKeyEncodingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="c7e0b-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="c7e0b-108">成员</span><span class="sxs-lookup"><span data-stu-id="c7e0b-108">Members</span></span>
|<span data-ttu-id="c7e0b-109">成员</span><span class="sxs-lookup"><span data-stu-id="c7e0b-109">Member</span></span>|<span data-ttu-id="c7e0b-110">值</span><span class="sxs-lookup"><span data-stu-id="c7e0b-110">Value</span></span>|<span data-ttu-id="c7e0b-111">说明</span><span class="sxs-lookup"><span data-stu-id="c7e0b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7e0b-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="c7e0b-112">deviceDefault</span></span>|<span data-ttu-id="c7e0b-113">0</span><span class="sxs-lookup"><span data-stu-id="c7e0b-113">0</span></span>|<span data-ttu-id="c7e0b-114">没有由 Intune 配置的值，请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="c7e0b-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="c7e0b-115">无</span><span class="sxs-lookup"><span data-stu-id="c7e0b-115">none</span></span>|<span data-ttu-id="c7e0b-116">1 </span><span class="sxs-lookup"><span data-stu-id="c7e0b-116">1</span></span>|<span data-ttu-id="c7e0b-117">未对预共享密钥进行编码。</span><span class="sxs-lookup"><span data-stu-id="c7e0b-117">Preshared key is not encoded.</span></span> <span data-ttu-id="c7e0b-118">相反，它将保留为其宽字符格式</span><span class="sxs-lookup"><span data-stu-id="c7e0b-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="c7e0b-119">utF8</span><span class="sxs-lookup"><span data-stu-id="c7e0b-119">utF8</span></span>|<span data-ttu-id="c7e0b-120">2 </span><span class="sxs-lookup"><span data-stu-id="c7e0b-120">2</span></span>|<span data-ttu-id="c7e0b-121">使用 UTF-8 对预共享密钥进行编码</span><span class="sxs-lookup"><span data-stu-id="c7e0b-121">Encode the preshared key using UTF-8</span></span>|



