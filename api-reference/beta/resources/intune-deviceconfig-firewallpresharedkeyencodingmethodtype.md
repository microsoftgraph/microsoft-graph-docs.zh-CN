---
title: firewallPreSharedKeyEncodingMethodType 枚举类型
description: FirewallPreSharedKeyEncodingMethod 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 513a6c545fedc73add4e710ed784ef223d1f8539
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976350"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="5dafd-103">firewallPreSharedKeyEncodingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5dafd-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="5dafd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5dafd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5dafd-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5dafd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5dafd-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5dafd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5dafd-107">FirewallPreSharedKeyEncodingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="5dafd-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="5dafd-108">成员</span><span class="sxs-lookup"><span data-stu-id="5dafd-108">Members</span></span>
|<span data-ttu-id="5dafd-109">成员</span><span class="sxs-lookup"><span data-stu-id="5dafd-109">Member</span></span>|<span data-ttu-id="5dafd-110">值</span><span class="sxs-lookup"><span data-stu-id="5dafd-110">Value</span></span>|<span data-ttu-id="5dafd-111">Description</span><span class="sxs-lookup"><span data-stu-id="5dafd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dafd-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="5dafd-112">deviceDefault</span></span>|<span data-ttu-id="5dafd-113">0</span><span class="sxs-lookup"><span data-stu-id="5dafd-113">0</span></span>|<span data-ttu-id="5dafd-114">配置通过 Intune，没有值不会替代的用户配置设备默认值</span><span class="sxs-lookup"><span data-stu-id="5dafd-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="5dafd-115">无</span><span class="sxs-lookup"><span data-stu-id="5dafd-115">none</span></span>|<span data-ttu-id="5dafd-116">1</span><span class="sxs-lookup"><span data-stu-id="5dafd-116">1</span></span>|<span data-ttu-id="5dafd-117">未编码预共享的密钥。</span><span class="sxs-lookup"><span data-stu-id="5dafd-117">Preshared key is not encoded.</span></span> <span data-ttu-id="5dafd-118">而是保留在其宽字符格式</span><span class="sxs-lookup"><span data-stu-id="5dafd-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="5dafd-119">utF8</span><span class="sxs-lookup"><span data-stu-id="5dafd-119">utF8</span></span>|<span data-ttu-id="5dafd-120">2</span><span class="sxs-lookup"><span data-stu-id="5dafd-120">2</span></span>|<span data-ttu-id="5dafd-121">预共享的密钥使用 utf-8 编码</span><span class="sxs-lookup"><span data-stu-id="5dafd-121">Encode the preshared key using UTF-8</span></span>|





