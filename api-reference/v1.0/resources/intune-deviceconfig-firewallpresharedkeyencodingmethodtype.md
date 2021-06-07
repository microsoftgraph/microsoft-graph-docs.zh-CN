---
title: firewallPreSharedKeyEncodingMethodType 枚举类型
description: firewallPreSharedKeyEncodingMethod 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 200177be7f8258965067f12cace3b163aefc6b78
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755054"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="ff291-103">firewallPreSharedKeyEncodingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ff291-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

<span data-ttu-id="ff291-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff291-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff291-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff291-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff291-106">firewallPreSharedKeyEncodingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="ff291-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="ff291-107">成员</span><span class="sxs-lookup"><span data-stu-id="ff291-107">Members</span></span>
|<span data-ttu-id="ff291-108">成员</span><span class="sxs-lookup"><span data-stu-id="ff291-108">Member</span></span>|<span data-ttu-id="ff291-109">值</span><span class="sxs-lookup"><span data-stu-id="ff291-109">Value</span></span>|<span data-ttu-id="ff291-110">Description</span><span class="sxs-lookup"><span data-stu-id="ff291-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff291-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="ff291-111">deviceDefault</span></span>|<span data-ttu-id="ff291-112">0</span><span class="sxs-lookup"><span data-stu-id="ff291-112">0</span></span>|<span data-ttu-id="ff291-113">Intune 未配置任何值，请勿替代用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="ff291-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="ff291-114">无</span><span class="sxs-lookup"><span data-stu-id="ff291-114">none</span></span>|<span data-ttu-id="ff291-115">1</span><span class="sxs-lookup"><span data-stu-id="ff291-115">1</span></span>|<span data-ttu-id="ff291-116">预共享密钥未进行编码。</span><span class="sxs-lookup"><span data-stu-id="ff291-116">Preshared key is not encoded.</span></span> <span data-ttu-id="ff291-117">相反，它保留为宽字符格式</span><span class="sxs-lookup"><span data-stu-id="ff291-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="ff291-118">utF8</span><span class="sxs-lookup"><span data-stu-id="ff291-118">utF8</span></span>|<span data-ttu-id="ff291-119">2</span><span class="sxs-lookup"><span data-stu-id="ff291-119">2</span></span>|<span data-ttu-id="ff291-120">使用 UTF-8 对预共享密钥进行编码</span><span class="sxs-lookup"><span data-stu-id="ff291-120">Encode the preshared key using UTF-8</span></span>|




