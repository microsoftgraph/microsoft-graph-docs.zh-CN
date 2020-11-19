---
title: keyStorageProviderOption 枚举类型
description: 密钥存储提供程序 (KSP) 导入选项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d0a0fca9dd77a4c83022d875350f12a3e56e18d6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301554"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="2f1f6-103">keyStorageProviderOption 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2f1f6-103">keyStorageProviderOption enum type</span></span>

<span data-ttu-id="2f1f6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f1f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f1f6-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2f1f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f1f6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f1f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f1f6-107">密钥存储提供程序 (KSP) 导入选项。</span><span class="sxs-lookup"><span data-stu-id="2f1f6-107">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="2f1f6-108">成员</span><span class="sxs-lookup"><span data-stu-id="2f1f6-108">Members</span></span>
|<span data-ttu-id="2f1f6-109">成员</span><span class="sxs-lookup"><span data-stu-id="2f1f6-109">Member</span></span>|<span data-ttu-id="2f1f6-110">值</span><span class="sxs-lookup"><span data-stu-id="2f1f6-110">Value</span></span>|<span data-ttu-id="2f1f6-111">说明</span><span class="sxs-lookup"><span data-stu-id="2f1f6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f1f6-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="2f1f6-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="2f1f6-113">0</span><span class="sxs-lookup"><span data-stu-id="2f1f6-113">0</span></span>|<span data-ttu-id="2f1f6-114">导入到受信任的平台模块 (TPM) KSP （如果存在），否则导入到软件 KSP。</span><span class="sxs-lookup"><span data-stu-id="2f1f6-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="2f1f6-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="2f1f6-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="2f1f6-116">1</span><span class="sxs-lookup"><span data-stu-id="2f1f6-116">1</span></span>|<span data-ttu-id="2f1f6-117">导入到受信任的平台模块 (TPM) KSP （如果存在），否则会失败。</span><span class="sxs-lookup"><span data-stu-id="2f1f6-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="2f1f6-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="2f1f6-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="2f1f6-119">双面</span><span class="sxs-lookup"><span data-stu-id="2f1f6-119">2</span></span>|<span data-ttu-id="2f1f6-120">导入 Passport for work KSP （如果可用），否则会失败。</span><span class="sxs-lookup"><span data-stu-id="2f1f6-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="2f1f6-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="2f1f6-121">useSoftwareKsp</span></span>|<span data-ttu-id="2f1f6-122">第三章</span><span class="sxs-lookup"><span data-stu-id="2f1f6-122">3</span></span>|<span data-ttu-id="2f1f6-123">导入到软件 KSP。</span><span class="sxs-lookup"><span data-stu-id="2f1f6-123">Import to Software KSP.</span></span>|




