---
title: firewallPreSharedKeyEncodingMethodType 枚举类型
description: FirewallPreSharedKeyEncodingMethod 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e6ad3214eb16e69c6a3da7aa51a69cc8b43eca90
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056679"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="0c5b5-103">firewallPreSharedKeyEncodingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0c5b5-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

<span data-ttu-id="0c5b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c5b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c5b5-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0c5b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c5b5-106">FirewallPreSharedKeyEncodingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="0c5b5-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="0c5b5-107">成员</span><span class="sxs-lookup"><span data-stu-id="0c5b5-107">Members</span></span>
|<span data-ttu-id="0c5b5-108">成员</span><span class="sxs-lookup"><span data-stu-id="0c5b5-108">Member</span></span>|<span data-ttu-id="0c5b5-109">值</span><span class="sxs-lookup"><span data-stu-id="0c5b5-109">Value</span></span>|<span data-ttu-id="0c5b5-110">说明</span><span class="sxs-lookup"><span data-stu-id="0c5b5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c5b5-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="0c5b5-111">deviceDefault</span></span>|<span data-ttu-id="0c5b5-112">0</span><span class="sxs-lookup"><span data-stu-id="0c5b5-112">0</span></span>|<span data-ttu-id="0c5b5-113">没有由 Intune 配置的值，请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="0c5b5-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="0c5b5-114">无</span><span class="sxs-lookup"><span data-stu-id="0c5b5-114">none</span></span>|<span data-ttu-id="0c5b5-115">1 </span><span class="sxs-lookup"><span data-stu-id="0c5b5-115">1</span></span>|<span data-ttu-id="0c5b5-116">未对预共享密钥进行编码。</span><span class="sxs-lookup"><span data-stu-id="0c5b5-116">Preshared key is not encoded.</span></span> <span data-ttu-id="0c5b5-117">相反，它将保留为其宽字符格式</span><span class="sxs-lookup"><span data-stu-id="0c5b5-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="0c5b5-118">utF8</span><span class="sxs-lookup"><span data-stu-id="0c5b5-118">utF8</span></span>|<span data-ttu-id="0c5b5-119">2 </span><span class="sxs-lookup"><span data-stu-id="0c5b5-119">2</span></span>|<span data-ttu-id="0c5b5-120">使用 UTF-8 对预共享密钥进行编码</span><span class="sxs-lookup"><span data-stu-id="0c5b5-120">Encode the preshared key using UTF-8</span></span>|









