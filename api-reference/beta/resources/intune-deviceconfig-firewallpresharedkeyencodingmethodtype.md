---
title: firewallPreSharedKeyEncodingMethodType 枚举类型
description: FirewallPreSharedKeyEncodingMethod 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 24407bb787e471340de8111fb6662b5f67ff610a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730635"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="038b1-103">firewallPreSharedKeyEncodingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="038b1-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

<span data-ttu-id="038b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="038b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="038b1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="038b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="038b1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="038b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="038b1-107">FirewallPreSharedKeyEncodingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="038b1-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="038b1-108">成员</span><span class="sxs-lookup"><span data-stu-id="038b1-108">Members</span></span>
|<span data-ttu-id="038b1-109">成员</span><span class="sxs-lookup"><span data-stu-id="038b1-109">Member</span></span>|<span data-ttu-id="038b1-110">值</span><span class="sxs-lookup"><span data-stu-id="038b1-110">Value</span></span>|<span data-ttu-id="038b1-111">说明</span><span class="sxs-lookup"><span data-stu-id="038b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="038b1-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="038b1-112">deviceDefault</span></span>|<span data-ttu-id="038b1-113">0</span><span class="sxs-lookup"><span data-stu-id="038b1-113">0</span></span>|<span data-ttu-id="038b1-114">没有由 Intune 配置的值，请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="038b1-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="038b1-115">无</span><span class="sxs-lookup"><span data-stu-id="038b1-115">none</span></span>|<span data-ttu-id="038b1-116">1</span><span class="sxs-lookup"><span data-stu-id="038b1-116">1</span></span>|<span data-ttu-id="038b1-117">未对预共享密钥进行编码。</span><span class="sxs-lookup"><span data-stu-id="038b1-117">Preshared key is not encoded.</span></span> <span data-ttu-id="038b1-118">相反，它将保留为其宽字符格式</span><span class="sxs-lookup"><span data-stu-id="038b1-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="038b1-119">utF8</span><span class="sxs-lookup"><span data-stu-id="038b1-119">utF8</span></span>|<span data-ttu-id="038b1-120">双面</span><span class="sxs-lookup"><span data-stu-id="038b1-120">2</span></span>|<span data-ttu-id="038b1-121">使用 UTF-8 对预共享密钥进行编码</span><span class="sxs-lookup"><span data-stu-id="038b1-121">Encode the preshared key using UTF-8</span></span>|





