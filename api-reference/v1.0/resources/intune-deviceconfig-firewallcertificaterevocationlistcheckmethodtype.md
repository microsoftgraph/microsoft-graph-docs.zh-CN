---
title: firewallCertificateRevocationListCheckMethodType 枚举类型
description: firewallCertificateRevocationListCheckMethod 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 779cfe8b8576d475df62ed112709aa0c2e9b6c63
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754725"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="0b6d1-103">firewallCertificateRevocationListCheckMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0b6d1-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="0b6d1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b6d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b6d1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0b6d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b6d1-106">firewallCertificateRevocationListCheckMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="0b6d1-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="0b6d1-107">成员</span><span class="sxs-lookup"><span data-stu-id="0b6d1-107">Members</span></span>
|<span data-ttu-id="0b6d1-108">成员</span><span class="sxs-lookup"><span data-stu-id="0b6d1-108">Member</span></span>|<span data-ttu-id="0b6d1-109">值</span><span class="sxs-lookup"><span data-stu-id="0b6d1-109">Value</span></span>|<span data-ttu-id="0b6d1-110">Description</span><span class="sxs-lookup"><span data-stu-id="0b6d1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b6d1-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="0b6d1-111">deviceDefault</span></span>|<span data-ttu-id="0b6d1-112">0</span><span class="sxs-lookup"><span data-stu-id="0b6d1-112">0</span></span>|<span data-ttu-id="0b6d1-113">Intune 未配置任何值，请勿替代用户配置的设备默认值</span><span class="sxs-lookup"><span data-stu-id="0b6d1-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="0b6d1-114">无</span><span class="sxs-lookup"><span data-stu-id="0b6d1-114">none</span></span>|<span data-ttu-id="0b6d1-115">1</span><span class="sxs-lookup"><span data-stu-id="0b6d1-115">1</span></span>|<span data-ttu-id="0b6d1-116">不检查证书吊销列表</span><span class="sxs-lookup"><span data-stu-id="0b6d1-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="0b6d1-117">attempt</span><span class="sxs-lookup"><span data-stu-id="0b6d1-117">attempt</span></span>|<span data-ttu-id="0b6d1-118">2</span><span class="sxs-lookup"><span data-stu-id="0b6d1-118">2</span></span>|<span data-ttu-id="0b6d1-119">仅在检查确认证书时，才尝试 CRL 检查并允许证书</span><span class="sxs-lookup"><span data-stu-id="0b6d1-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="0b6d1-120">require</span><span class="sxs-lookup"><span data-stu-id="0b6d1-120">require</span></span>|<span data-ttu-id="0b6d1-121">3</span><span class="sxs-lookup"><span data-stu-id="0b6d1-121">3</span></span>|<span data-ttu-id="0b6d1-122">在允许证书之前需要成功的 CRL 检查</span><span class="sxs-lookup"><span data-stu-id="0b6d1-122">Require a successful CRL check before allowing a certificate</span></span>|




