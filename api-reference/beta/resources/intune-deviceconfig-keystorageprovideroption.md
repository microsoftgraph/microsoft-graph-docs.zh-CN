---
title: keyStorageProviderOption 枚举类型
description: 密钥存储提供程序 (KSP) 导入选项。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ddc1cffe1f4e6056d53a151a3b36b2622c9bf4b5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153016"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="5ea5e-103">keyStorageProviderOption 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5ea5e-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="5ea5e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5ea5e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ea5e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5ea5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ea5e-106">密钥存储提供程序 (KSP) 导入选项。</span><span class="sxs-lookup"><span data-stu-id="5ea5e-106">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="5ea5e-107">成员</span><span class="sxs-lookup"><span data-stu-id="5ea5e-107">Members</span></span>
|<span data-ttu-id="5ea5e-108">成员</span><span class="sxs-lookup"><span data-stu-id="5ea5e-108">Member</span></span>|<span data-ttu-id="5ea5e-109">值</span><span class="sxs-lookup"><span data-stu-id="5ea5e-109">Value</span></span>|<span data-ttu-id="5ea5e-110">说明</span><span class="sxs-lookup"><span data-stu-id="5ea5e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ea5e-111">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="5ea5e-111">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="5ea5e-112">0</span><span class="sxs-lookup"><span data-stu-id="5ea5e-112">0</span></span>|<span data-ttu-id="5ea5e-113">导入到受信任的平台模块 (TPM) KSP (如果存在), 否则导入到软件 KSP。</span><span class="sxs-lookup"><span data-stu-id="5ea5e-113">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="5ea5e-114">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="5ea5e-114">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="5ea5e-115">1</span><span class="sxs-lookup"><span data-stu-id="5ea5e-115">1</span></span>|<span data-ttu-id="5ea5e-116">导入到受信任的平台模块 (TPM) KSP (如果存在), 否则会失败。</span><span class="sxs-lookup"><span data-stu-id="5ea5e-116">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="5ea5e-117">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="5ea5e-117">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="5ea5e-118">双面</span><span class="sxs-lookup"><span data-stu-id="5ea5e-118">2</span></span>|<span data-ttu-id="5ea5e-119">导入 Passport for work KSP (如果可用), 否则会失败。</span><span class="sxs-lookup"><span data-stu-id="5ea5e-119">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="5ea5e-120">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="5ea5e-120">useSoftwareKsp</span></span>|<span data-ttu-id="5ea5e-121">第三章</span><span class="sxs-lookup"><span data-stu-id="5ea5e-121">3</span></span>|<span data-ttu-id="5ea5e-122">导入到软件 KSP。</span><span class="sxs-lookup"><span data-stu-id="5ea5e-122">Import to Software KSP.</span></span>|




