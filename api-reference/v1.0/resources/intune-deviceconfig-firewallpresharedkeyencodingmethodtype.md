---
title: firewallPreSharedKeyEncodingMethodType 枚举类型
description: firewallPreSharedKeyEncodingMethod 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c62144ef2974da5a3d975c759bb8d2bd2be6032
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541176"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="12d49-103">firewallPreSharedKeyEncodingMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="12d49-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="12d49-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12d49-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12d49-105">firewallPreSharedKeyEncodingMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="12d49-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="12d49-106">成员</span><span class="sxs-lookup"><span data-stu-id="12d49-106">Members</span></span>
|<span data-ttu-id="12d49-107">成员</span><span class="sxs-lookup"><span data-stu-id="12d49-107">Member</span></span>|<span data-ttu-id="12d49-108">值</span><span class="sxs-lookup"><span data-stu-id="12d49-108">Value</span></span>|<span data-ttu-id="12d49-109">说明</span><span class="sxs-lookup"><span data-stu-id="12d49-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12d49-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="12d49-110">deviceDefault</span></span>|<span data-ttu-id="12d49-111">0</span><span class="sxs-lookup"><span data-stu-id="12d49-111">0</span></span>|<span data-ttu-id="12d49-112">没有由 Intune 配置的值, 请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="12d49-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="12d49-113">无</span><span class="sxs-lookup"><span data-stu-id="12d49-113">none</span></span>|<span data-ttu-id="12d49-114">1</span><span class="sxs-lookup"><span data-stu-id="12d49-114">1</span></span>|<span data-ttu-id="12d49-115">未对预共享密钥进行编码。</span><span class="sxs-lookup"><span data-stu-id="12d49-115">Preshared key is not encoded.</span></span> <span data-ttu-id="12d49-116">相反, 它将保留为其宽字符格式</span><span class="sxs-lookup"><span data-stu-id="12d49-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="12d49-117">utF8</span><span class="sxs-lookup"><span data-stu-id="12d49-117">utF8</span></span>|<span data-ttu-id="12d49-118">2 </span><span class="sxs-lookup"><span data-stu-id="12d49-118">2</span></span>|<span data-ttu-id="12d49-119">使用 utf-8 对预共享密钥进行编码</span><span class="sxs-lookup"><span data-stu-id="12d49-119">Encode the preshared key using UTF-8</span></span>|



