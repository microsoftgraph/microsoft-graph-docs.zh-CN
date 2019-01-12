---
title: firewallPreSharedKeyEncodingMethodType 枚举类型
description: FirewallPreSharedKeyEncodingMethod 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4ad59a11aec2fbf715657de95eb3aafc778da43a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947825"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="1f483-103">firewallPreSharedKeyEncodingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1f483-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="1f483-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1f483-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f483-105">FirewallPreSharedKeyEncodingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="1f483-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="1f483-106">成员</span><span class="sxs-lookup"><span data-stu-id="1f483-106">Members</span></span>
|<span data-ttu-id="1f483-107">成员</span><span class="sxs-lookup"><span data-stu-id="1f483-107">Member</span></span>|<span data-ttu-id="1f483-108">值</span><span class="sxs-lookup"><span data-stu-id="1f483-108">Value</span></span>|<span data-ttu-id="1f483-109">说明</span><span class="sxs-lookup"><span data-stu-id="1f483-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f483-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="1f483-110">deviceDefault</span></span>|<span data-ttu-id="1f483-111">0</span><span class="sxs-lookup"><span data-stu-id="1f483-111">0</span></span>|<span data-ttu-id="1f483-112">配置通过 Intune，没有值不会替代的用户配置设备默认值</span><span class="sxs-lookup"><span data-stu-id="1f483-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="1f483-113">无</span><span class="sxs-lookup"><span data-stu-id="1f483-113">none</span></span>|<span data-ttu-id="1f483-114">1</span><span class="sxs-lookup"><span data-stu-id="1f483-114">1</span></span>|<span data-ttu-id="1f483-115">未编码预共享的密钥。</span><span class="sxs-lookup"><span data-stu-id="1f483-115">Preshared key is not encoded.</span></span> <span data-ttu-id="1f483-116">而是保留在其宽字符格式</span><span class="sxs-lookup"><span data-stu-id="1f483-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="1f483-117">utF8</span><span class="sxs-lookup"><span data-stu-id="1f483-117">utF8</span></span>|<span data-ttu-id="1f483-118">2</span><span class="sxs-lookup"><span data-stu-id="1f483-118">2</span></span>|<span data-ttu-id="1f483-119">预共享的密钥使用 utf-8 编码</span><span class="sxs-lookup"><span data-stu-id="1f483-119">Encode the preshared key using UTF-8</span></span>|



