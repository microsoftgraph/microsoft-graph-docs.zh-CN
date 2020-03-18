---
title: emailCertificateType 枚举类型
description: 支持的电子邮件签名和加密的证书来源。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7dbf484473643eff30463cb8c4dc8217113ab713
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791812"
---
# <a name="emailcertificatetype-enum-type"></a><span data-ttu-id="8fffc-103">emailCertificateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8fffc-103">emailCertificateType enum type</span></span>

> <span data-ttu-id="8fffc-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8fffc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fffc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8fffc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fffc-106">支持的电子邮件签名和加密的证书来源。</span><span class="sxs-lookup"><span data-stu-id="8fffc-106">Supported certificate sources for email signing and encryption.</span></span>

## <a name="members"></a><span data-ttu-id="8fffc-107">成员</span><span class="sxs-lookup"><span data-stu-id="8fffc-107">Members</span></span>
|<span data-ttu-id="8fffc-108">成员</span><span class="sxs-lookup"><span data-stu-id="8fffc-108">Member</span></span>|<span data-ttu-id="8fffc-109">值</span><span class="sxs-lookup"><span data-stu-id="8fffc-109">Value</span></span>|<span data-ttu-id="8fffc-110">说明</span><span class="sxs-lookup"><span data-stu-id="8fffc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fffc-111">无</span><span class="sxs-lookup"><span data-stu-id="8fffc-111">none</span></span>|<span data-ttu-id="8fffc-112">0</span><span class="sxs-lookup"><span data-stu-id="8fffc-112">0</span></span>|<span data-ttu-id="8fffc-113">不要将证书用作源。</span><span class="sxs-lookup"><span data-stu-id="8fffc-113">Do not use a certificate as a source.</span></span>|
|<span data-ttu-id="8fffc-114">证书</span><span class="sxs-lookup"><span data-stu-id="8fffc-114">certificate</span></span>|<span data-ttu-id="8fffc-115">1</span><span class="sxs-lookup"><span data-stu-id="8fffc-115">1</span></span>|<span data-ttu-id="8fffc-116">对证书源使用证书。</span><span class="sxs-lookup"><span data-stu-id="8fffc-116">Use an certificate for certificate source.</span></span>|
|<span data-ttu-id="8fffc-117">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="8fffc-117">derivedCredential</span></span>|<span data-ttu-id="8fffc-118">双面</span><span class="sxs-lookup"><span data-stu-id="8fffc-118">2</span></span>|<span data-ttu-id="8fffc-119">对证书源使用派生凭据。</span><span class="sxs-lookup"><span data-stu-id="8fffc-119">Use a derived credential for certificate source.</span></span>|



