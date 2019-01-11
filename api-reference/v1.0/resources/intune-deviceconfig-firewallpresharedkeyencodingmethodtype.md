---
title: firewallPreSharedKeyEncodingMethodType 枚举类型
description: FirewallPreSharedKeyEncodingMethod 的可能值
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bba6033985f2b960a272134614d98acc7203a9d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871748"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="539c1-103">firewallPreSharedKeyEncodingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="539c1-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="539c1-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="539c1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="539c1-105">FirewallPreSharedKeyEncodingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="539c1-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="539c1-106">成员</span><span class="sxs-lookup"><span data-stu-id="539c1-106">Members</span></span>
|<span data-ttu-id="539c1-107">成员</span><span class="sxs-lookup"><span data-stu-id="539c1-107">Member</span></span>|<span data-ttu-id="539c1-108">值</span><span class="sxs-lookup"><span data-stu-id="539c1-108">Value</span></span>|<span data-ttu-id="539c1-109">Description</span><span class="sxs-lookup"><span data-stu-id="539c1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="539c1-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="539c1-110">deviceDefault</span></span>|<span data-ttu-id="539c1-111">0</span><span class="sxs-lookup"><span data-stu-id="539c1-111">0</span></span>|<span data-ttu-id="539c1-112">配置通过 Intune，没有值不会替代的用户配置设备默认值</span><span class="sxs-lookup"><span data-stu-id="539c1-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="539c1-113">无</span><span class="sxs-lookup"><span data-stu-id="539c1-113">none</span></span>|<span data-ttu-id="539c1-114">1</span><span class="sxs-lookup"><span data-stu-id="539c1-114">1</span></span>|<span data-ttu-id="539c1-115">未编码预共享的密钥。</span><span class="sxs-lookup"><span data-stu-id="539c1-115">Preshared key is not encoded.</span></span> <span data-ttu-id="539c1-116">而是保留在其宽字符格式</span><span class="sxs-lookup"><span data-stu-id="539c1-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="539c1-117">utF8</span><span class="sxs-lookup"><span data-stu-id="539c1-117">utF8</span></span>|<span data-ttu-id="539c1-118">2</span><span class="sxs-lookup"><span data-stu-id="539c1-118">2</span></span>|<span data-ttu-id="539c1-119">预共享的密钥使用 utf-8 编码</span><span class="sxs-lookup"><span data-stu-id="539c1-119">Encode the preshared key using UTF-8</span></span>|



