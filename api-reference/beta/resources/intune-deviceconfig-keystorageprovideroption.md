---
title: keyStorageProviderOption 枚举类型
description: 密钥存储提供程序 (KSP) 导入选项。
author: tfitzmac
ms.openlocfilehash: 7923dd5c4b8a09d834d29b65928430828f3dafac
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342215"
---
# <a name="keystorageprovideroption-enum-type"></a><span data-ttu-id="4ecd6-103">keyStorageProviderOption 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4ecd6-103">keyStorageProviderOption enum type</span></span>

> <span data-ttu-id="4ecd6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4ecd6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ecd6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4ecd6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4ecd6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4ecd6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ecd6-107">密钥存储提供程序 (KSP) 导入选项。</span><span class="sxs-lookup"><span data-stu-id="4ecd6-107">Key Storage Provider (KSP) Import Options.</span></span>
## <a name="members"></a><span data-ttu-id="4ecd6-108">成员</span><span class="sxs-lookup"><span data-stu-id="4ecd6-108">Members</span></span>
|<span data-ttu-id="4ecd6-109">成员</span><span class="sxs-lookup"><span data-stu-id="4ecd6-109">Member</span></span>|<span data-ttu-id="4ecd6-110">值</span><span class="sxs-lookup"><span data-stu-id="4ecd6-110">Value</span></span>|<span data-ttu-id="4ecd6-111">说明</span><span class="sxs-lookup"><span data-stu-id="4ecd6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ecd6-112">useTpmKspOtherwiseUseSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="4ecd6-112">useTpmKspOtherwiseUseSoftwareKsp</span></span>|<span data-ttu-id="4ecd6-113">0</span><span class="sxs-lookup"><span data-stu-id="4ecd6-113">0</span></span>|<span data-ttu-id="4ecd6-114">导入到受信任平台模块 (TPM) KSP 如果存在此参数，否则导入到软件 KSP。</span><span class="sxs-lookup"><span data-stu-id="4ecd6-114">Import to Trusted Platform Module (TPM) KSP if present, otherwise import to Software KSP.</span></span>|
|<span data-ttu-id="4ecd6-115">useTpmKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="4ecd6-115">useTpmKspOtherwiseFail</span></span>|<span data-ttu-id="4ecd6-116">1</span><span class="sxs-lookup"><span data-stu-id="4ecd6-116">1</span></span>|<span data-ttu-id="4ecd6-117">导入到受信任平台模块 (TPM) KSP 如果存在此参数，否则会失败。</span><span class="sxs-lookup"><span data-stu-id="4ecd6-117">Import to Trusted Platform Module (TPM) KSP if present, otherwise fail.</span></span>|
|<span data-ttu-id="4ecd6-118">usePassportForWorkKspOtherwiseFail</span><span class="sxs-lookup"><span data-stu-id="4ecd6-118">usePassportForWorkKspOtherwiseFail</span></span>|<span data-ttu-id="4ecd6-119">2</span><span class="sxs-lookup"><span data-stu-id="4ecd6-119">2</span></span>|<span data-ttu-id="4ecd6-120">导入到 Passport 工作 KSP 如果可用，否则失败。</span><span class="sxs-lookup"><span data-stu-id="4ecd6-120">Import to Passport for work KSP if available, otherwise fail.</span></span>|
|<span data-ttu-id="4ecd6-121">useSoftwareKsp</span><span class="sxs-lookup"><span data-stu-id="4ecd6-121">useSoftwareKsp</span></span>|<span data-ttu-id="4ecd6-122">3</span><span class="sxs-lookup"><span data-stu-id="4ecd6-122">3</span></span>|<span data-ttu-id="4ecd6-123">导入到软件 KSP。</span><span class="sxs-lookup"><span data-stu-id="4ecd6-123">Import to Software KSP.</span></span>|





