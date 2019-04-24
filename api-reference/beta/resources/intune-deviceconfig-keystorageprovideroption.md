---
title: keyStorageProviderOption 枚举类型
description: 密钥存储提供程序 (KSP) 导入选项。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b422443abcdb72cd76399ae9f2e0fea59bb6f34f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460420"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="e4a21-103">keyStorageProviderOption 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e4a21-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="e4a21-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e4a21-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4a21-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e4a21-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4a21-106">密钥存储提供程序 (KSP) 导入选项。</span><span class="sxs-lookup"><span data-stu-id="e4a21-106">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="e4a21-107">成员</span><span class="sxs-lookup"><span data-stu-id="e4a21-107">Members</span></span>
|<span data-ttu-id="e4a21-108">成员</span><span class="sxs-lookup"><span data-stu-id="e4a21-108">Member</span></span>|<span data-ttu-id="e4a21-109">值</span><span class="sxs-lookup"><span data-stu-id="e4a21-109">Value</span></span>|<span data-ttu-id="e4a21-110">说明</span><span class="sxs-lookup"><span data-stu-id="e4a21-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4a21-111">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="e4a21-111">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="e4a21-112">0</span><span class="sxs-lookup"><span data-stu-id="e4a21-112">0</span></span>|<span data-ttu-id="e4a21-113">导入到受信任的平台模块 (TPM) KSP (如果存在), 否则导入到软件 KSP。</span><span class="sxs-lookup"><span data-stu-id="e4a21-113">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="e4a21-114">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="e4a21-114">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="e4a21-115">1</span><span class="sxs-lookup"><span data-stu-id="e4a21-115">1</span></span>|<span data-ttu-id="e4a21-116">导入到受信任的平台模块 (TPM) KSP (如果存在), 否则会失败。</span><span class="sxs-lookup"><span data-stu-id="e4a21-116">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="e4a21-117">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="e4a21-117">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="e4a21-118">2 </span><span class="sxs-lookup"><span data-stu-id="e4a21-118">2</span></span>|<span data-ttu-id="e4a21-119">导入 Passport for work KSP (如果可用), 否则会失败。</span><span class="sxs-lookup"><span data-stu-id="e4a21-119">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="e4a21-120">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="e4a21-120">useSoftwareKsp</span></span>|<span data-ttu-id="e4a21-121">3 </span><span class="sxs-lookup"><span data-stu-id="e4a21-121">3</span></span>|<span data-ttu-id="e4a21-122">导入到软件 KSP。</span><span class="sxs-lookup"><span data-stu-id="e4a21-122">Import to Software KSP.</span></span>|





