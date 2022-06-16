---
title: Microsoft Graph 数据连接概述
description: 使用 Microsoft Graph 数据连接大规模访问 Microsoft 365 批量数据、启用精细许可并提供数据安全性和管理。
author: fercobo-msft
ms.localizationpriority: high
ms.prod: data-connect
ms.custom: scenarios:getting-started
ms.openlocfilehash: 2870f56b2c784bba233fc2db9accac12f13e82d2
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094044"
---
# <a name="overview-of-microsoft-graph-data-connect"></a>Microsoft Graph 数据连接概述

Microsoft Graph 数据连接通过智能方式大规模访问丰富数据，增强了 Microsoft Graph 的事务性模型。 这些数据涵盖员工如何在 Microsoft 365 中的所有应用程序和服务之间进行沟通、协作和管理时间。 

数据连接是大数据和机器学习的理想选择，让你能够通过将 Microsoft 365 数据扩展到 Azure 来开发用于分析、智能和业务流程优化的应用程序。 通过以这种方式集成，你将能够利用 Azure 中的大量计算、存储套件，同时保持符合行业标准并确保数据安全。

![图像显示在 Azure 云中的 Microsoft 365 数据和输出数据之间应用的数据控制。](images/data-connect-mgdc-capabilities.png)

Microsoft Graph 数据连接使用 Azure 数据工厂以可配置的时间间隔将 Microsoft 365 数据复制到应用程序的存储中。 它还提供了一组工具来简化向 Microsoft Azure 传送此数据的过程，让你可以访问最适用的开发和托管工具。 

数据连接还授权更精细的控制和同意模型：你可以管理数据，查看谁正在访问数据以及请求实体的特定属性。 这增强了 Microsoft Graph 模型，其授予或拒绝应用程序对整个实体的访问权限。

可以使用“数据连接”来为组织实现机器学习的场景。在这些方案中，可以创建应用程序来为利益干系人提供宝贵信息、训练机器学习模型，甚至根据采集的大量数据进行预测。</br>

<!--<iframe class="video-iframe" style="width: 960px; height: 540px;" frameborder="0" allowfullscreen="true" src="https://www.microsoft.com/en-us/videoplayer/embed/RWEJsy?autoplay=false"> </iframe>-->

> [!VIDEO https://www.microsoft.com/en-us/videoplayer/embed/RWEJsy?autoplay=false]

如果你同意 [Microsoft API 使用条款](/legal/microsoft-apis/terms-of-use?context=/graph/context)和 [Microsoft 隐私声明](https://go.microsoft.com/fwlink/p/?LinkId=123161)，并且是下述人员之一，则可利用 Microsoft Graph 数据连接：

- 一个 ISV，它用于为所有 Microsoft 365 客户构建智能应用程序。
- 一名企业开发人员，他为组织内部用户构建可访问 Microsoft 365 数据的智能应用程序。

## <a name="access-to-data-at-scale"></a>大规模访问数据

丰富的应用程序需要访问大量数据，通常来自于组织中许多用户同时进行访问。 因此，Microsoft Graph 的标准事务数据模型倾向于限制大型数据集。 数据交付需要复杂的基础结构和数千个 API 调用，其中任何一项都可能由于资源限制而被限制。 

Microsoft Graph 数据连接通过批量访问数据并使用 Azure 数据工厂重复将 Microsoft 365 数据复制到你的应用程序来解决这一难题。 通过数据连接，你还能够选择访问组织中每个人的数据还是仅访问特定人员组的数据。

## <a name="granular-data-consent"></a>精细数据同意

在传统的 Microsoft Graph 同意模型中，管理员或用户只能授予或拒绝应用程序访问特定的预定义实体集的请求。 例如，对 Mail.Read 的请求包含对支持 Outlook 邮件的固定实体集的读取访问权限，其中包括具有其所有相关属性的整个 [message](/graph/api/resources/message) 实例。 

Microsoft Graph 数据连接支持更精细的同意，允许应用程序请求访问实体中的特定属性，或筛选这些属性中的数据。 管理员必须先明确批准才能访问 Microsoft Graph 数据。 请求必须指定所请求的访问权限的级别、数据策略实施、请求的原因以及所请求数据的架构。 因此，应用程序只能使用对其功能运行至关重要的数据，并排除任何不相关的内容。 例如，应用可使用电子邮件元数据，但排除正文内容和附件。

## <a name="data-security-and-governance"></a>数据安全性和管理

Microsoft 正在促使 Microsoft Graph 数据连接和 Azure 之间就客户数据进行丰富的连接通信。 数据连接支持所有 Azure 本机服务功能，例如加密、地理围栏、审核和策略实施。 

为了最大程度减少你使用数据连接构建的应用的合规性管理开销，你可以指定一组要遵循的详细策略，Microsoft 365 管理员随后可审阅这些策略。 在这些策略获准后，Microsoft 将监控应用程序对策略的遵循情况。 如果应用程序违反（或试图违反）组织建立的策略，Microsoft 将停止向该应用程序传输数据。

## <a name="see-also"></a>另请参阅

- [构建第一个 Microsoft Graph 数据连接应用程序教程](data-connect-quickstart.yml)。
- [数据连接常见问题解答](data-connect-faq.md)
- [数据集、区域和接收器](data-connect-datasets.md)
