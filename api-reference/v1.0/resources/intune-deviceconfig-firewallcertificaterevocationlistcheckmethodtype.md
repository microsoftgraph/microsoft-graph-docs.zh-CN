---
title: firewallCertificateRevocationListCheckMethodType 枚举类型
description: FirewallCertificateRevocationListCheckMethod 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 969a94ed8a782989aaf9d34c00fe1f4cc82775ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056707"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="10795-103">firewallCertificateRevocationListCheckMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="10795-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="10795-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10795-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10795-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="10795-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10795-106">FirewallCertificateRevocationListCheckMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="10795-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="10795-107">成员</span><span class="sxs-lookup"><span data-stu-id="10795-107">Members</span></span>
|<span data-ttu-id="10795-108">成员</span><span class="sxs-lookup"><span data-stu-id="10795-108">Member</span></span>|<span data-ttu-id="10795-109">值</span><span class="sxs-lookup"><span data-stu-id="10795-109">Value</span></span>|<span data-ttu-id="10795-110">说明</span><span class="sxs-lookup"><span data-stu-id="10795-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10795-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="10795-111">deviceDefault</span></span>|<span data-ttu-id="10795-112">0</span><span class="sxs-lookup"><span data-stu-id="10795-112">0</span></span>|<span data-ttu-id="10795-113">没有由 Intune 配置的值，请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="10795-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="10795-114">无</span><span class="sxs-lookup"><span data-stu-id="10795-114">none</span></span>|<span data-ttu-id="10795-115">1 </span><span class="sxs-lookup"><span data-stu-id="10795-115">1</span></span>|<span data-ttu-id="10795-116">不检查证书吊销列表</span><span class="sxs-lookup"><span data-stu-id="10795-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="10795-117">应试</span><span class="sxs-lookup"><span data-stu-id="10795-117">attempt</span></span>|<span data-ttu-id="10795-118">2 </span><span class="sxs-lookup"><span data-stu-id="10795-118">2</span></span>|<span data-ttu-id="10795-119">仅当支票确认证书时，才尝试 CRL 检查并允许证书</span><span class="sxs-lookup"><span data-stu-id="10795-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="10795-120">无须</span><span class="sxs-lookup"><span data-stu-id="10795-120">require</span></span>|<span data-ttu-id="10795-121">第三章</span><span class="sxs-lookup"><span data-stu-id="10795-121">3</span></span>|<span data-ttu-id="10795-122">在允许证书之前，需要进行成功的 CRL 检查</span><span class="sxs-lookup"><span data-stu-id="10795-122">Require a successful CRL check before allowing a certificate</span></span>|









