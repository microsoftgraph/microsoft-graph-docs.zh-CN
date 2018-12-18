---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型
description: 凭据 Guard 设置的可能值。
author: tfitzmac
ms.openlocfilehash: 6f6c952d1c480d42db45de6345eba883ff5848a8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346961"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="32a3b-103">deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="32a3b-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="32a3b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="32a3b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32a3b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="32a3b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="32a3b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="32a3b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32a3b-107">凭据 Guard 设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="32a3b-107">Possible values of Credential Guard settings.</span></span>
## <a name="members"></a><span data-ttu-id="32a3b-108">成员</span><span class="sxs-lookup"><span data-stu-id="32a3b-108">Members</span></span>
|<span data-ttu-id="32a3b-109">成员</span><span class="sxs-lookup"><span data-stu-id="32a3b-109">Member</span></span>|<span data-ttu-id="32a3b-110">值</span><span class="sxs-lookup"><span data-stu-id="32a3b-110">Value</span></span>|<span data-ttu-id="32a3b-111">说明</span><span class="sxs-lookup"><span data-stu-id="32a3b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32a3b-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="32a3b-112">notConfigured</span></span>|<span data-ttu-id="32a3b-113">0</span><span class="sxs-lookup"><span data-stu-id="32a3b-113">0</span></span>|<span data-ttu-id="32a3b-114">关闭凭据 Guard 远程如果没有 UEFI 锁定之前配置。</span><span class="sxs-lookup"><span data-stu-id="32a3b-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="32a3b-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="32a3b-115">enableWithUEFILock</span></span>|<span data-ttu-id="32a3b-116">1</span><span class="sxs-lookup"><span data-stu-id="32a3b-116">1</span></span>|<span data-ttu-id="32a3b-117">打开与 UEFI 锁定凭据 Guard。</span><span class="sxs-lookup"><span data-stu-id="32a3b-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="32a3b-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="32a3b-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="32a3b-119">2</span><span class="sxs-lookup"><span data-stu-id="32a3b-119">2</span></span>|<span data-ttu-id="32a3b-120">UEFI 锁定的情况下启用凭据 Guard。</span><span class="sxs-lookup"><span data-stu-id="32a3b-120">Turns on Credential Guard without UEFI lock.</span></span>|





