---
title: firewallPreSharedKeyEncodingMethodType 枚举类型
description: firewallPreSharedKeyEncodingMethod 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36c49a0c97ac8f2e9267f20762fd6e748d952240
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556184"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="19e8a-103">firewallPreSharedKeyEncodingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="19e8a-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="19e8a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="19e8a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19e8a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="19e8a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19e8a-106">firewallPreSharedKeyEncodingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="19e8a-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="19e8a-107">成员</span><span class="sxs-lookup"><span data-stu-id="19e8a-107">Members</span></span>
|<span data-ttu-id="19e8a-108">成员</span><span class="sxs-lookup"><span data-stu-id="19e8a-108">Member</span></span>|<span data-ttu-id="19e8a-109">值</span><span class="sxs-lookup"><span data-stu-id="19e8a-109">Value</span></span>|<span data-ttu-id="19e8a-110">说明</span><span class="sxs-lookup"><span data-stu-id="19e8a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19e8a-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="19e8a-111">deviceDefault</span></span>|<span data-ttu-id="19e8a-112">0</span><span class="sxs-lookup"><span data-stu-id="19e8a-112">0</span></span>|<span data-ttu-id="19e8a-113">没有由 Intune 配置的值, 请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="19e8a-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="19e8a-114">无</span><span class="sxs-lookup"><span data-stu-id="19e8a-114">none</span></span>|<span data-ttu-id="19e8a-115">1</span><span class="sxs-lookup"><span data-stu-id="19e8a-115">1</span></span>|<span data-ttu-id="19e8a-116">未对预共享密钥进行编码。</span><span class="sxs-lookup"><span data-stu-id="19e8a-116">Preshared key is not encoded.</span></span> <span data-ttu-id="19e8a-117">相反, 它将保留为其宽字符格式</span><span class="sxs-lookup"><span data-stu-id="19e8a-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="19e8a-118">utF8</span><span class="sxs-lookup"><span data-stu-id="19e8a-118">utF8</span></span>|<span data-ttu-id="19e8a-119">2 </span><span class="sxs-lookup"><span data-stu-id="19e8a-119">2</span></span>|<span data-ttu-id="19e8a-120">使用 utf-8 对预共享密钥进行编码</span><span class="sxs-lookup"><span data-stu-id="19e8a-120">Encode the preshared key using UTF-8</span></span>|





