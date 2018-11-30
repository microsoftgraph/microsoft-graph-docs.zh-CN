---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型
description: 凭据 Guard 设置的可能值。
ms.openlocfilehash: 73668ec4d6d5026402757fae3443da4540fb374c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041522"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="78c72-103">deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="78c72-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="78c72-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="78c72-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78c72-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="78c72-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78c72-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="78c72-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78c72-107">凭据 Guard 设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="78c72-107">Possible values of Credential Guard settings.</span></span>
## <a name="members"></a><span data-ttu-id="78c72-108">成员</span><span class="sxs-lookup"><span data-stu-id="78c72-108">Members</span></span>
|<span data-ttu-id="78c72-109">成员</span><span class="sxs-lookup"><span data-stu-id="78c72-109">Member</span></span>|<span data-ttu-id="78c72-110">值</span><span class="sxs-lookup"><span data-stu-id="78c72-110">Value</span></span>|<span data-ttu-id="78c72-111">说明</span><span class="sxs-lookup"><span data-stu-id="78c72-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78c72-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="78c72-112">notConfigured</span></span>|<span data-ttu-id="78c72-113">0</span><span class="sxs-lookup"><span data-stu-id="78c72-113">0</span></span>|<span data-ttu-id="78c72-114">关闭凭据 Guard 远程如果没有 UEFI 锁定之前配置。</span><span class="sxs-lookup"><span data-stu-id="78c72-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="78c72-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="78c72-115">enableWithUEFILock</span></span>|<span data-ttu-id="78c72-116">1</span><span class="sxs-lookup"><span data-stu-id="78c72-116">1</span></span>|<span data-ttu-id="78c72-117">打开与 UEFI 锁定凭据 Guard。</span><span class="sxs-lookup"><span data-stu-id="78c72-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="78c72-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="78c72-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="78c72-119">2</span><span class="sxs-lookup"><span data-stu-id="78c72-119">2</span></span>|<span data-ttu-id="78c72-120">UEFI 锁定的情况下启用凭据 Guard。</span><span class="sxs-lookup"><span data-stu-id="78c72-120">Turns on Credential Guard without UEFI lock.</span></span>|





