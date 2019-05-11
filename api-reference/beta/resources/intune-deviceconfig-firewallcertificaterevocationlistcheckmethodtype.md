---
title: firewallCertificateRevocationListCheckMethodType 枚举类型
description: FirewallCertificateRevocationListCheckMethod 的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 92d0f13416e543e018a5a69d28751d9ddd4512c8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946635"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="37c58-103">firewallCertificateRevocationListCheckMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="37c58-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="37c58-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="37c58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37c58-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="37c58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37c58-106">FirewallCertificateRevocationListCheckMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="37c58-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="37c58-107">成员</span><span class="sxs-lookup"><span data-stu-id="37c58-107">Members</span></span>
|<span data-ttu-id="37c58-108">成员</span><span class="sxs-lookup"><span data-stu-id="37c58-108">Member</span></span>|<span data-ttu-id="37c58-109">值</span><span class="sxs-lookup"><span data-stu-id="37c58-109">Value</span></span>|<span data-ttu-id="37c58-110">说明</span><span class="sxs-lookup"><span data-stu-id="37c58-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37c58-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="37c58-111">deviceDefault</span></span>|<span data-ttu-id="37c58-112">0</span><span class="sxs-lookup"><span data-stu-id="37c58-112">0</span></span>|<span data-ttu-id="37c58-113">没有由 Intune 配置的值, 请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="37c58-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="37c58-114">无</span><span class="sxs-lookup"><span data-stu-id="37c58-114">none</span></span>|<span data-ttu-id="37c58-115">1</span><span class="sxs-lookup"><span data-stu-id="37c58-115">1</span></span>|<span data-ttu-id="37c58-116">不检查证书吊销列表</span><span class="sxs-lookup"><span data-stu-id="37c58-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="37c58-117">应试</span><span class="sxs-lookup"><span data-stu-id="37c58-117">attempt</span></span>|<span data-ttu-id="37c58-118">双面</span><span class="sxs-lookup"><span data-stu-id="37c58-118">2</span></span>|<span data-ttu-id="37c58-119">仅当支票确认证书时, 才尝试 CRL 检查并允许证书</span><span class="sxs-lookup"><span data-stu-id="37c58-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="37c58-120">无须</span><span class="sxs-lookup"><span data-stu-id="37c58-120">require</span></span>|<span data-ttu-id="37c58-121">第三章</span><span class="sxs-lookup"><span data-stu-id="37c58-121">3</span></span>|<span data-ttu-id="37c58-122">在允许证书之前, 需要进行成功的 CRL 检查</span><span class="sxs-lookup"><span data-stu-id="37c58-122">Require a successful CRL check before allowing a certificate</span></span>|




