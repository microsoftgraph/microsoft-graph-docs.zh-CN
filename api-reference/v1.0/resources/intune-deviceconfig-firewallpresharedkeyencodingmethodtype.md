---
title: firewallPreSharedKeyEncodingMethodType 枚举类型
description: FirewallPreSharedKeyEncodingMethod 的可能值
author: tfitzmac
ms.openlocfilehash: b8ab119c58aec6e62c0a32ccf310f43eab029573
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343587"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="393cc-103">firewallPreSharedKeyEncodingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="393cc-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="393cc-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="393cc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="393cc-105">FirewallPreSharedKeyEncodingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="393cc-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="393cc-106">成员</span><span class="sxs-lookup"><span data-stu-id="393cc-106">Members</span></span>
|<span data-ttu-id="393cc-107">成员</span><span class="sxs-lookup"><span data-stu-id="393cc-107">Member</span></span>|<span data-ttu-id="393cc-108">值</span><span class="sxs-lookup"><span data-stu-id="393cc-108">Value</span></span>|<span data-ttu-id="393cc-109">说明</span><span class="sxs-lookup"><span data-stu-id="393cc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="393cc-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="393cc-110">deviceDefault</span></span>|<span data-ttu-id="393cc-111">0</span><span class="sxs-lookup"><span data-stu-id="393cc-111">0</span></span>|<span data-ttu-id="393cc-112">配置通过 Intune，没有值不会替代的用户配置设备默认值</span><span class="sxs-lookup"><span data-stu-id="393cc-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="393cc-113">无</span><span class="sxs-lookup"><span data-stu-id="393cc-113">none</span></span>|<span data-ttu-id="393cc-114">1</span><span class="sxs-lookup"><span data-stu-id="393cc-114">1</span></span>|<span data-ttu-id="393cc-115">未编码预共享的密钥。</span><span class="sxs-lookup"><span data-stu-id="393cc-115">Preshared key is not encoded.</span></span> <span data-ttu-id="393cc-116">而是保留在其宽字符格式</span><span class="sxs-lookup"><span data-stu-id="393cc-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="393cc-117">utF8</span><span class="sxs-lookup"><span data-stu-id="393cc-117">utF8</span></span>|<span data-ttu-id="393cc-118">2</span><span class="sxs-lookup"><span data-stu-id="393cc-118">2</span></span>|<span data-ttu-id="393cc-119">预共享的密钥使用 utf-8 编码</span><span class="sxs-lookup"><span data-stu-id="393cc-119">Encode the preshared key using UTF-8</span></span>|



