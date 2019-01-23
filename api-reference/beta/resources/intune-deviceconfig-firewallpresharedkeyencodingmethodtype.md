---
title: firewallPreSharedKeyEncodingMethodType 枚举类型
description: FirewallPreSharedKeyEncodingMethod 的可能值
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 577925f141c6dd94b493664d3617df939d19c5c6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410950"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="342e8-103">firewallPreSharedKeyEncodingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="342e8-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="342e8-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="342e8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="342e8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="342e8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="342e8-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="342e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="342e8-107">FirewallPreSharedKeyEncodingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="342e8-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="342e8-108">成员</span><span class="sxs-lookup"><span data-stu-id="342e8-108">Members</span></span>
|<span data-ttu-id="342e8-109">成员</span><span class="sxs-lookup"><span data-stu-id="342e8-109">Member</span></span>|<span data-ttu-id="342e8-110">值</span><span class="sxs-lookup"><span data-stu-id="342e8-110">Value</span></span>|<span data-ttu-id="342e8-111">说明</span><span class="sxs-lookup"><span data-stu-id="342e8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="342e8-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="342e8-112">deviceDefault</span></span>|<span data-ttu-id="342e8-113">0</span><span class="sxs-lookup"><span data-stu-id="342e8-113">0</span></span>|<span data-ttu-id="342e8-114">配置通过 Intune，没有值不会替代的用户配置设备默认值</span><span class="sxs-lookup"><span data-stu-id="342e8-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="342e8-115">无</span><span class="sxs-lookup"><span data-stu-id="342e8-115">none</span></span>|<span data-ttu-id="342e8-116">1</span><span class="sxs-lookup"><span data-stu-id="342e8-116">1</span></span>|<span data-ttu-id="342e8-117">未编码预共享的密钥。</span><span class="sxs-lookup"><span data-stu-id="342e8-117">Preshared key is not encoded.</span></span> <span data-ttu-id="342e8-118">而是保留在其宽字符格式</span><span class="sxs-lookup"><span data-stu-id="342e8-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="342e8-119">utF8</span><span class="sxs-lookup"><span data-stu-id="342e8-119">utF8</span></span>|<span data-ttu-id="342e8-120">2</span><span class="sxs-lookup"><span data-stu-id="342e8-120">2</span></span>|<span data-ttu-id="342e8-121">预共享的密钥使用 utf-8 编码</span><span class="sxs-lookup"><span data-stu-id="342e8-121">Encode the preshared key using UTF-8</span></span>|




