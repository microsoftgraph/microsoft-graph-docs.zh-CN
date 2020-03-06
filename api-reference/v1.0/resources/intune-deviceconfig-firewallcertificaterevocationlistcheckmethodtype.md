---
title: firewallCertificateRevocationListCheckMethodType 枚举类型
description: FirewallCertificateRevocationListCheckMethod 的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1eeda2493b91e63d54a45c89ed0f840288f97f43
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532526"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="a748f-103">firewallCertificateRevocationListCheckMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a748f-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="a748f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a748f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a748f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a748f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a748f-106">FirewallCertificateRevocationListCheckMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="a748f-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="a748f-107">成员</span><span class="sxs-lookup"><span data-stu-id="a748f-107">Members</span></span>
|<span data-ttu-id="a748f-108">成员</span><span class="sxs-lookup"><span data-stu-id="a748f-108">Member</span></span>|<span data-ttu-id="a748f-109">值</span><span class="sxs-lookup"><span data-stu-id="a748f-109">Value</span></span>|<span data-ttu-id="a748f-110">说明</span><span class="sxs-lookup"><span data-stu-id="a748f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a748f-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="a748f-111">deviceDefault</span></span>|<span data-ttu-id="a748f-112">0</span><span class="sxs-lookup"><span data-stu-id="a748f-112">0</span></span>|<span data-ttu-id="a748f-113">没有由 Intune 配置的值，请勿覆盖用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="a748f-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="a748f-114">无</span><span class="sxs-lookup"><span data-stu-id="a748f-114">none</span></span>|<span data-ttu-id="a748f-115">1 </span><span class="sxs-lookup"><span data-stu-id="a748f-115">1</span></span>|<span data-ttu-id="a748f-116">不检查证书吊销列表</span><span class="sxs-lookup"><span data-stu-id="a748f-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="a748f-117">应试</span><span class="sxs-lookup"><span data-stu-id="a748f-117">attempt</span></span>|<span data-ttu-id="a748f-118">2 </span><span class="sxs-lookup"><span data-stu-id="a748f-118">2</span></span>|<span data-ttu-id="a748f-119">仅当支票确认证书时，才尝试 CRL 检查并允许证书</span><span class="sxs-lookup"><span data-stu-id="a748f-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="a748f-120">无须</span><span class="sxs-lookup"><span data-stu-id="a748f-120">require</span></span>|<span data-ttu-id="a748f-121">3 </span><span class="sxs-lookup"><span data-stu-id="a748f-121">3</span></span>|<span data-ttu-id="a748f-122">在允许证书之前，需要进行成功的 CRL 检查</span><span class="sxs-lookup"><span data-stu-id="a748f-122">Require a successful CRL check before allowing a certificate</span></span>|




