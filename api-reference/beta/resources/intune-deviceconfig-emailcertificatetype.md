---
title: emailCertificateType 枚举类型
description: 支持的电子邮件签名和加密的证书来源。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3d94c2a50542eb4d97a19fdb4ca0e1de2dcabf17
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49303305"
---
# <a name="emailcertificatetype-enum-type"></a><span data-ttu-id="cc3af-103">emailCertificateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cc3af-103">emailCertificateType enum type</span></span>

<span data-ttu-id="cc3af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc3af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc3af-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cc3af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc3af-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cc3af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc3af-107">支持的电子邮件签名和加密的证书来源。</span><span class="sxs-lookup"><span data-stu-id="cc3af-107">Supported certificate sources for email signing and encryption.</span></span>

## <a name="members"></a><span data-ttu-id="cc3af-108">成员</span><span class="sxs-lookup"><span data-stu-id="cc3af-108">Members</span></span>
|<span data-ttu-id="cc3af-109">成员</span><span class="sxs-lookup"><span data-stu-id="cc3af-109">Member</span></span>|<span data-ttu-id="cc3af-110">值</span><span class="sxs-lookup"><span data-stu-id="cc3af-110">Value</span></span>|<span data-ttu-id="cc3af-111">Description</span><span class="sxs-lookup"><span data-stu-id="cc3af-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc3af-112">无</span><span class="sxs-lookup"><span data-stu-id="cc3af-112">none</span></span>|<span data-ttu-id="cc3af-113">0</span><span class="sxs-lookup"><span data-stu-id="cc3af-113">0</span></span>|<span data-ttu-id="cc3af-114">不要将证书用作源。</span><span class="sxs-lookup"><span data-stu-id="cc3af-114">Do not use a certificate as a source.</span></span>|
|<span data-ttu-id="cc3af-115">证书</span><span class="sxs-lookup"><span data-stu-id="cc3af-115">certificate</span></span>|<span data-ttu-id="cc3af-116">1</span><span class="sxs-lookup"><span data-stu-id="cc3af-116">1</span></span>|<span data-ttu-id="cc3af-117">对证书源使用证书。</span><span class="sxs-lookup"><span data-stu-id="cc3af-117">Use an certificate for certificate source.</span></span>|
|<span data-ttu-id="cc3af-118">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="cc3af-118">derivedCredential</span></span>|<span data-ttu-id="cc3af-119">双面</span><span class="sxs-lookup"><span data-stu-id="cc3af-119">2</span></span>|<span data-ttu-id="cc3af-120">对证书源使用派生凭据。</span><span class="sxs-lookup"><span data-stu-id="cc3af-120">Use a derived credential for certificate source.</span></span>|




