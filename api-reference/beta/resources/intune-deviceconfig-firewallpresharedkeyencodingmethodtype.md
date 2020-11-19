---
title: firewallPreSharedKeyEncodingMethodType 枚举类型
description: FirewallPreSharedKeyEncodingMethod 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 79fcb89a8165cbea6d2132eda256c742231fd129
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49303214"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="dbb08-103">firewallPreSharedKeyEncodingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="dbb08-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

<span data-ttu-id="dbb08-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbb08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dbb08-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dbb08-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dbb08-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dbb08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbb08-107">FirewallPreSharedKeyEncodingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="dbb08-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="dbb08-108">成员</span><span class="sxs-lookup"><span data-stu-id="dbb08-108">Members</span></span>
|<span data-ttu-id="dbb08-109">成员</span><span class="sxs-lookup"><span data-stu-id="dbb08-109">Member</span></span>|<span data-ttu-id="dbb08-110">值</span><span class="sxs-lookup"><span data-stu-id="dbb08-110">Value</span></span>|<span data-ttu-id="dbb08-111">Description</span><span class="sxs-lookup"><span data-stu-id="dbb08-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbb08-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="dbb08-112">deviceDefault</span></span>|<span data-ttu-id="dbb08-113">0</span><span class="sxs-lookup"><span data-stu-id="dbb08-113">0</span></span>|<span data-ttu-id="dbb08-114">没有由 Intune 配置的值，请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="dbb08-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="dbb08-115">无</span><span class="sxs-lookup"><span data-stu-id="dbb08-115">none</span></span>|<span data-ttu-id="dbb08-116">1</span><span class="sxs-lookup"><span data-stu-id="dbb08-116">1</span></span>|<span data-ttu-id="dbb08-117">未对预共享密钥进行编码。</span><span class="sxs-lookup"><span data-stu-id="dbb08-117">Preshared key is not encoded.</span></span> <span data-ttu-id="dbb08-118">相反，它将保留为其宽字符格式</span><span class="sxs-lookup"><span data-stu-id="dbb08-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="dbb08-119">utF8</span><span class="sxs-lookup"><span data-stu-id="dbb08-119">utF8</span></span>|<span data-ttu-id="dbb08-120">双面</span><span class="sxs-lookup"><span data-stu-id="dbb08-120">2</span></span>|<span data-ttu-id="dbb08-121">使用 UTF-8 对预共享密钥进行编码</span><span class="sxs-lookup"><span data-stu-id="dbb08-121">Encode the preshared key using UTF-8</span></span>|




