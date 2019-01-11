---
title: keyStorageProviderOption 枚举类型
description: 密钥存储提供程序 (KSP) 导入选项。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4609092c3022b62331bbb6226a5b91e4b287ff79
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826465"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="7806f-103">keyStorageProviderOption 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7806f-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="7806f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7806f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7806f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7806f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7806f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7806f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7806f-107">密钥存储提供程序 (KSP) 导入选项。</span><span class="sxs-lookup"><span data-stu-id="7806f-107">Key Storage Provider (KSP) Import Options.</span></span>
## <a name="members"></a><span data-ttu-id="7806f-108">成员</span><span class="sxs-lookup"><span data-stu-id="7806f-108">Members</span></span>
|<span data-ttu-id="7806f-109">成员</span><span class="sxs-lookup"><span data-stu-id="7806f-109">Member</span></span>|<span data-ttu-id="7806f-110">值</span><span class="sxs-lookup"><span data-stu-id="7806f-110">Value</span></span>|<span data-ttu-id="7806f-111">Description</span><span class="sxs-lookup"><span data-stu-id="7806f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7806f-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="7806f-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="7806f-113">0</span><span class="sxs-lookup"><span data-stu-id="7806f-113">0</span></span>|<span data-ttu-id="7806f-114">导入到受信任平台模块 (TPM) KSP 如果存在此参数，否则导入到软件 KSP。</span><span class="sxs-lookup"><span data-stu-id="7806f-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="7806f-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="7806f-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="7806f-116">1</span><span class="sxs-lookup"><span data-stu-id="7806f-116">1</span></span>|<span data-ttu-id="7806f-117">导入到受信任平台模块 (TPM) KSP 如果存在此参数，否则会失败。</span><span class="sxs-lookup"><span data-stu-id="7806f-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="7806f-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="7806f-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="7806f-119">2</span><span class="sxs-lookup"><span data-stu-id="7806f-119">2</span></span>|<span data-ttu-id="7806f-120">导入到 Passport 工作 KSP 如果可用，否则失败。</span><span class="sxs-lookup"><span data-stu-id="7806f-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="7806f-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="7806f-121">useSoftwareKsp</span></span>|<span data-ttu-id="7806f-122">3</span><span class="sxs-lookup"><span data-stu-id="7806f-122">3</span></span>|<span data-ttu-id="7806f-123">导入到软件 KSP。</span><span class="sxs-lookup"><span data-stu-id="7806f-123">Import to Software KSP.</span></span>|





