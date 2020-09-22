---
title: emailCertificateType 枚举类型
description: 支持的电子邮件签名和加密的证书来源。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b5fe1392d09576de4d0154d941d87293f87615bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095259"
---
# <a name="emailcertificatetype-enum-type"></a><span data-ttu-id="3748f-103">emailCertificateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3748f-103">emailCertificateType enum type</span></span>

<span data-ttu-id="3748f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3748f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3748f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3748f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3748f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3748f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3748f-107">支持的电子邮件签名和加密的证书来源。</span><span class="sxs-lookup"><span data-stu-id="3748f-107">Supported certificate sources for email signing and encryption.</span></span>

## <a name="members"></a><span data-ttu-id="3748f-108">成员</span><span class="sxs-lookup"><span data-stu-id="3748f-108">Members</span></span>
|<span data-ttu-id="3748f-109">成员</span><span class="sxs-lookup"><span data-stu-id="3748f-109">Member</span></span>|<span data-ttu-id="3748f-110">值</span><span class="sxs-lookup"><span data-stu-id="3748f-110">Value</span></span>|<span data-ttu-id="3748f-111">说明</span><span class="sxs-lookup"><span data-stu-id="3748f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3748f-112">无</span><span class="sxs-lookup"><span data-stu-id="3748f-112">none</span></span>|<span data-ttu-id="3748f-113">0</span><span class="sxs-lookup"><span data-stu-id="3748f-113">0</span></span>|<span data-ttu-id="3748f-114">不要将证书用作源。</span><span class="sxs-lookup"><span data-stu-id="3748f-114">Do not use a certificate as a source.</span></span>|
|<span data-ttu-id="3748f-115">证书</span><span class="sxs-lookup"><span data-stu-id="3748f-115">certificate</span></span>|<span data-ttu-id="3748f-116">1 </span><span class="sxs-lookup"><span data-stu-id="3748f-116">1</span></span>|<span data-ttu-id="3748f-117">对证书源使用证书。</span><span class="sxs-lookup"><span data-stu-id="3748f-117">Use an certificate for certificate source.</span></span>|
|<span data-ttu-id="3748f-118">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="3748f-118">derivedCredential</span></span>|<span data-ttu-id="3748f-119">2 </span><span class="sxs-lookup"><span data-stu-id="3748f-119">2</span></span>|<span data-ttu-id="3748f-120">对证书源使用派生凭据。</span><span class="sxs-lookup"><span data-stu-id="3748f-120">Use a derived credential for certificate source.</span></span>|






