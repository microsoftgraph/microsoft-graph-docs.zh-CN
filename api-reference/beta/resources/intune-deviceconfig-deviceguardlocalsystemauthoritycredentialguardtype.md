---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型
description: 凭据 Guard 设置的可能值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8d8643744e1f5c36cf6c620ac85a6a99c9a77548
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398091"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="dec47-103">deviceGuardLocalSystemAuthorityCredentialGuardType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="dec47-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="dec47-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="dec47-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dec47-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dec47-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dec47-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dec47-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dec47-107">凭据 Guard 设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="dec47-107">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="dec47-108">成员</span><span class="sxs-lookup"><span data-stu-id="dec47-108">Members</span></span>
|<span data-ttu-id="dec47-109">成员</span><span class="sxs-lookup"><span data-stu-id="dec47-109">Member</span></span>|<span data-ttu-id="dec47-110">值</span><span class="sxs-lookup"><span data-stu-id="dec47-110">Value</span></span>|<span data-ttu-id="dec47-111">说明</span><span class="sxs-lookup"><span data-stu-id="dec47-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dec47-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="dec47-112">notConfigured</span></span>|<span data-ttu-id="dec47-113">0</span><span class="sxs-lookup"><span data-stu-id="dec47-113">0</span></span>|<span data-ttu-id="dec47-114">关闭凭据 Guard 远程如果没有 UEFI 锁定之前配置。</span><span class="sxs-lookup"><span data-stu-id="dec47-114">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="dec47-115">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="dec47-115">enableWithUEFILock</span></span>|<span data-ttu-id="dec47-116">1</span><span class="sxs-lookup"><span data-stu-id="dec47-116">1</span></span>|<span data-ttu-id="dec47-117">打开与 UEFI 锁定凭据 Guard。</span><span class="sxs-lookup"><span data-stu-id="dec47-117">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="dec47-118">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="dec47-118">enableWithoutUEFILock</span></span>|<span data-ttu-id="dec47-119">2</span><span class="sxs-lookup"><span data-stu-id="dec47-119">2</span></span>|<span data-ttu-id="dec47-120">UEFI 锁定的情况下启用凭据 Guard。</span><span class="sxs-lookup"><span data-stu-id="dec47-120">Turns on Credential Guard without UEFI lock.</span></span>|




