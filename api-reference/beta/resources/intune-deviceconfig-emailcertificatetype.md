---
title: emailCertificateType 枚举类型
description: 支持的电子邮件签名和加密的证书来源。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a2ff58f55033660a839a5f28d0244217c62936e0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996384"
---
# <a name="emailcertificatetype-enum-type"></a><span data-ttu-id="616e7-103">emailCertificateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="616e7-103">emailCertificateType enum type</span></span>

> <span data-ttu-id="616e7-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="616e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="616e7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="616e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="616e7-106">支持的电子邮件签名和加密的证书来源。</span><span class="sxs-lookup"><span data-stu-id="616e7-106">Supported certificate sources for email signing and encryption.</span></span>

## <a name="members"></a><span data-ttu-id="616e7-107">成员</span><span class="sxs-lookup"><span data-stu-id="616e7-107">Members</span></span>
|<span data-ttu-id="616e7-108">成员</span><span class="sxs-lookup"><span data-stu-id="616e7-108">Member</span></span>|<span data-ttu-id="616e7-109">值</span><span class="sxs-lookup"><span data-stu-id="616e7-109">Value</span></span>|<span data-ttu-id="616e7-110">说明</span><span class="sxs-lookup"><span data-stu-id="616e7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="616e7-111">无</span><span class="sxs-lookup"><span data-stu-id="616e7-111">none</span></span>|<span data-ttu-id="616e7-112">0</span><span class="sxs-lookup"><span data-stu-id="616e7-112">0</span></span>|<span data-ttu-id="616e7-113">不要将证书用作源。</span><span class="sxs-lookup"><span data-stu-id="616e7-113">Do not use a certificate as a source.</span></span>|
|<span data-ttu-id="616e7-114">证书</span><span class="sxs-lookup"><span data-stu-id="616e7-114">certificate</span></span>|<span data-ttu-id="616e7-115">1</span><span class="sxs-lookup"><span data-stu-id="616e7-115">1</span></span>|<span data-ttu-id="616e7-116">对证书源使用证书。</span><span class="sxs-lookup"><span data-stu-id="616e7-116">Use an certificate for certificate source.</span></span>|
|<span data-ttu-id="616e7-117">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="616e7-117">derivedCredential</span></span>|<span data-ttu-id="616e7-118">双面</span><span class="sxs-lookup"><span data-stu-id="616e7-118">2</span></span>|<span data-ttu-id="616e7-119">对证书源使用派生凭据。</span><span class="sxs-lookup"><span data-stu-id="616e7-119">Use a derived credential for certificate source.</span></span>|





