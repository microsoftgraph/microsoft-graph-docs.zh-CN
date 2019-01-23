---
title: keyStorageProviderOption 枚举类型
description: 密钥存储提供程序 (KSP) 导入选项。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6993d7e241ef94c572975c709c286a14f6eabf5b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424222"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="8ba28-103">keyStorageProviderOption 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8ba28-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="8ba28-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="8ba28-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8ba28-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8ba28-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8ba28-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8ba28-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ba28-107">密钥存储提供程序 (KSP) 导入选项。</span><span class="sxs-lookup"><span data-stu-id="8ba28-107">Key Storage Provider (KSP) Import Options.</span></span>

## <a name="members"></a><span data-ttu-id="8ba28-108">成员</span><span class="sxs-lookup"><span data-stu-id="8ba28-108">Members</span></span>
|<span data-ttu-id="8ba28-109">成员</span><span class="sxs-lookup"><span data-stu-id="8ba28-109">Member</span></span>|<span data-ttu-id="8ba28-110">值</span><span class="sxs-lookup"><span data-stu-id="8ba28-110">Value</span></span>|<span data-ttu-id="8ba28-111">说明</span><span class="sxs-lookup"><span data-stu-id="8ba28-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ba28-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="8ba28-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="8ba28-113">0</span><span class="sxs-lookup"><span data-stu-id="8ba28-113">0</span></span>|<span data-ttu-id="8ba28-114">导入到受信任平台模块 (TPM) KSP 如果存在此参数，否则导入到软件 KSP。</span><span class="sxs-lookup"><span data-stu-id="8ba28-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="8ba28-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="8ba28-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="8ba28-116">1</span><span class="sxs-lookup"><span data-stu-id="8ba28-116">1</span></span>|<span data-ttu-id="8ba28-117">导入到受信任平台模块 (TPM) KSP 如果存在此参数，否则会失败。</span><span class="sxs-lookup"><span data-stu-id="8ba28-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="8ba28-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="8ba28-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="8ba28-119">2</span><span class="sxs-lookup"><span data-stu-id="8ba28-119">2</span></span>|<span data-ttu-id="8ba28-120">导入到 Passport 工作 KSP 如果可用，否则失败。</span><span class="sxs-lookup"><span data-stu-id="8ba28-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="8ba28-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="8ba28-121">useSoftwareKsp</span></span>|<span data-ttu-id="8ba28-122">3</span><span class="sxs-lookup"><span data-stu-id="8ba28-122">3</span></span>|<span data-ttu-id="8ba28-123">导入到软件 KSP。</span><span class="sxs-lookup"><span data-stu-id="8ba28-123">Import to Software KSP.</span></span>|




