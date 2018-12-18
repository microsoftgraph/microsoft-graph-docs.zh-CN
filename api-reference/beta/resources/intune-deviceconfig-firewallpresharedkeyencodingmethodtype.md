---
title: firewallPreSharedKeyEncodingMethodType 枚举类型
description: FirewallPreSharedKeyEncodingMethod 的可能值
author: tfitzmac
ms.openlocfilehash: 3ed2456f54bd27a3efa04d959edba48f7c100692
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324931"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="da38d-103">firewallPreSharedKeyEncodingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="da38d-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="da38d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="da38d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da38d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="da38d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da38d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="da38d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da38d-107">FirewallPreSharedKeyEncodingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="da38d-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="da38d-108">成员</span><span class="sxs-lookup"><span data-stu-id="da38d-108">Members</span></span>
|<span data-ttu-id="da38d-109">成员</span><span class="sxs-lookup"><span data-stu-id="da38d-109">Member</span></span>|<span data-ttu-id="da38d-110">值</span><span class="sxs-lookup"><span data-stu-id="da38d-110">Value</span></span>|<span data-ttu-id="da38d-111">说明</span><span class="sxs-lookup"><span data-stu-id="da38d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da38d-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="da38d-112">deviceDefault</span></span>|<span data-ttu-id="da38d-113">0</span><span class="sxs-lookup"><span data-stu-id="da38d-113">0</span></span>|<span data-ttu-id="da38d-114">配置通过 Intune，没有值不会替代的用户配置设备默认值</span><span class="sxs-lookup"><span data-stu-id="da38d-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="da38d-115">无</span><span class="sxs-lookup"><span data-stu-id="da38d-115">none</span></span>|<span data-ttu-id="da38d-116">1</span><span class="sxs-lookup"><span data-stu-id="da38d-116">1</span></span>|<span data-ttu-id="da38d-117">未编码预共享的密钥。</span><span class="sxs-lookup"><span data-stu-id="da38d-117">Preshared key is not encoded.</span></span> <span data-ttu-id="da38d-118">而是保留在其宽字符格式</span><span class="sxs-lookup"><span data-stu-id="da38d-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="da38d-119">utF8</span><span class="sxs-lookup"><span data-stu-id="da38d-119">utF8</span></span>|<span data-ttu-id="da38d-120">2</span><span class="sxs-lookup"><span data-stu-id="da38d-120">2</span></span>|<span data-ttu-id="da38d-121">预共享的密钥使用 utf-8 编码</span><span class="sxs-lookup"><span data-stu-id="da38d-121">Encode the preshared key using UTF-8</span></span>|





