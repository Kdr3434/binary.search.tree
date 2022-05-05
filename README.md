{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "name": "Binary Search Tree Projesi",
      "provenance": [],
      "authorship_tag": "ABX9TyOc0WhV3MmeqhsNPAGvhpsc",
      "include_colab_link": true
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    },
    "language_info": {
      "name": "python"
    }
  },
  "cells": [
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "view-in-github",
        "colab_type": "text"
      },
      "source": [
        "<a href=\"https://colab.research.google.com/github/Murataltundag/murat/blob/main/Binary_Search_Tree_Projesi.ipynb\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
      ]
    },
    {
      "cell_type": "code",
      "execution_count": null,
      "metadata": {
        "id": "NEo0Y3ohpF8R"
      },
      "outputs": [],
      "source": [
        "def binary_search(item_list,item):\n",
        "\tfirst = 0\n",
        "\tlast = len(item_list)-1\n",
        "\tfound = False\n",
        "\twhile( first<=last and not found):\n",
        "\t\tmid = (first + last)//2\n",
        "\t\tif item_list[mid] == item :\n",
        "\t\t\tfound = True\n",
        "\t\telse:\n",
        "\t\t\tif item < item_list[mid]:\n",
        "\t\t\t\tlast = mid - 1\n",
        "\t\t\telse:\n",
        "\t\t\t\tfirst = mid + 1\t\n",
        "\treturn found\n",
        "\t\n",
        "\n",
        "arr = [7,5,1,8,3,6,0,9,4,2]\n",
        "x =1\n",
        "\n",
        "print(binary_search(arr,x))"
      ]
    }
  ]
}
