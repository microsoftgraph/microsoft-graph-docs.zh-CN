---
title: emailCertificateType 枚举类型
description: 支持的电子邮件签名和加密的证书来源。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 266bc9e0b23009f34281c70095176ccd88b50907
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526470"
---
# <a name="emailcertificatetype-enum-type"></a><span data-ttu-id="e4c66-103">emailCertificateType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e4c66-103">emailCertificateType enum type</span></span>

<span data-ttu-id="e4c66-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e4c66-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4c66-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e4c66-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4c66-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e4c66-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4c66-107">支持的电子邮件签名和加密的证书来源。</span><span class="sxs-lookup"><span data-stu-id="e4c66-107">Supported certificate sources for email signing and encryption.</span></span>

## <a name="members"></a><span data-ttu-id="e4c66-108">成员</span><span class="sxs-lookup"><span data-stu-id="e4c66-108">Members</span></span>
|<span data-ttu-id="e4c66-109">成员</span><span class="sxs-lookup"><span data-stu-id="e4c66-109">Member</span></span>|<span data-ttu-id="e4c66-110">值</span><span class="sxs-lookup"><span data-stu-id="e4c66-110">Value</span></span>|<span data-ttu-id="e4c66-111">说明</span><span class="sxs-lookup"><span data-stu-id="e4c66-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4c66-112">无</span><span class="sxs-lookup"><span data-stu-id="e4c66-112">none</span></span>|<span data-ttu-id="e4c66-113">0</span><span class="sxs-lookup"><span data-stu-id="e4c66-113">0</span></span>|<span data-ttu-id="e4c66-114">不要将证书用作源。</span><span class="sxs-lookup"><span data-stu-id="e4c66-114">Do not use a certificate as a source.</span></span>|
|<span data-ttu-id="e4c66-115">证书</span><span class="sxs-lookup"><span data-stu-id="e4c66-115">certificate</span></span>|<span data-ttu-id="e4c66-116">1 </span><span class="sxs-lookup"><span data-stu-id="e4c66-116">1</span></span>|<span data-ttu-id="e4c66-117">对证书源使用证书。</span><span class="sxs-lookup"><span data-stu-id="e4c66-117">Use an certificate for certificate source.</span></span>|
|<span data-ttu-id="e4c66-118">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="e4c66-118">derivedCredential</span></span>|<span data-ttu-id="e4c66-119">2 </span><span class="sxs-lookup"><span data-stu-id="e4c66-119">2</span></span>|<span data-ttu-id="e4c66-120">对证书源使用派生凭据。</span><span class="sxs-lookup"><span data-stu-id="e4c66-120">Use a derived credential for certificate source.</span></span>|



